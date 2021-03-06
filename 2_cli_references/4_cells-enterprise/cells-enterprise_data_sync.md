## ./cells-enterprise data sync

Trigger index resync

### Synopsis


Trigger a re-indexation of a given service. 
This can be currently used for datasource indexes and search engine.

```
./cells-enterprise data sync [flags]
```

### Examples

```
For example, to trigger the re-indexation of "pydiods1" datasource, target the "sync" service associated to the datasource : 

1) by name:
	./cells data sync --datasource=pydiods1

2) by service name:
	./cells data sync --service=pydio.grpc.data.sync.pydiods1 

Else to refresh the search engine entirely:
	./cells data sync --service=pydio.grpc.search --path=/
```

### Options

```
      --datasource string   Name of datasource to resync
  -h, --help                help for sync
      --path string         Path to resync (default "/")
      --service string      If no datasource name is passed, use the complete service name to resync
```

### Options inherited from parent commands

```
      --broker string                     Pub/sub service for events between services (currently nats only) (default "nats")
      --broker_address string             Broker port (default ":4222")
      --enable_metrics                    Instrument code to expose internal metrics
      --enable_pprof                      Enable pprof remote debugging
      --fork                              Used internally by application when forking processes
      --grpc_cert string                  Certificates used for communication via grpc
      --grpc_external string              External port exposed for gRPC (may be fixed if no SSL is configured or a reverse proxy is used)
      --grpc_key string                   Certificates used for communication via grpc
      --log string                        Sets the log level mode (default "info")
      --registry string                   Registry used to manage services (currently nats only) (default "nats")
      --registry_address string           Registry connection address (default ":4222")
      --registry_cluster_address string   Registry cluster address (default ":5222")
      --registry_cluster_routes string    Registry cluster routes
      --transport string                  Transport protocol for RPC (default "grpc")
      --transport_address string          Transport protocol port (default ":4222")
```

### SEE ALSO

* [./cells-enterprise data](./cells-enterprise-data)	 - Directly interact with a datasource

###### Auto generated by Pydio Cells Enterprise Distribution v2.1.5 on 31-Aug-2020
