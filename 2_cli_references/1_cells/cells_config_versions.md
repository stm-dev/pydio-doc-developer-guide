## ./cells config versions

List all configurations versions

### Synopsis


This command allows to manage configurations changes history and revert to a given version if necessary.

A version is created at each call to config.Save() inside the application, along with a log message
and the user originating this call.


```
./cells config versions [flags]
```

### Options

```
      --cat string       Print the JSON content of the config for this version
      --diff string      Display a Diff between two versions, either by providing VERSION1:VERSION2 or just VERSION1 (will be compared to previous one)
      --file string      Point to a specific DB file instead of default
  -h, --help             help for versions
      --restore string   Restore configuration to this specific version
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

* [./cells config](./cells-config)	 - Configuration manager

###### Auto generated by Pydio Cells Home Edition v2.1.5 on 31-Aug-2020
