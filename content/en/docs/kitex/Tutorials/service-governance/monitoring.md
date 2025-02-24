---
title: "Monitoring"
date: 2021-08-31
weight: 2
keywords: ["Kitex", "Monitoring", "Tracer"]
description: Kitex has monitoring capability built in, but does not have any monitoring features itself, and can be extended by the interface.
---

The framework provides a `Tracer` interface. Users can implement it and inject it by `WithTracer` Option.

```go
// Tracer is executed at the start and finish of an RPC.
type Tracer interface {
    Start(ctx context.Context) context.Context
    Finish(ctx context.Context)
}
```

The monitoring extension of prometheus is provided in [kitex-contrib](https://github.com/kitex-contrib/monitor-prometheus), usage example:

Client Side:

```go
import (
    "github.com/kitex-contrib/monitor-prometheus"
    kClient "github.com/cloudwego/kitex/client"
)

...

client, _ := testClient.NewClient(
    "DestServiceName",
    kClient.WithTracer(prometheus.NewClientTracer(":9091", "/kitexclient")))

resp, _ := client.Send(ctx, req)

...
```

Server Side:

```go
import (
    "github.com/kitex-contrib/monitor-prometheus"
    kServer "github.com/cloudwego/kitex/server"
)
func main() {...
    svr := xxxservice.NewServer(
        &myServiceImpl{},
        kServer.WithTracer(prometheus.NewServerTracer(":9092", "/kitexserver")))
    svr.Run()
    
    ...
}
```

