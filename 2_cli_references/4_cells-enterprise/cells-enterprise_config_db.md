## ./cells-enterprise config db

Manage Database configuration

### Synopsis

Manage Database configuration

```
./cells-enterprise config db [flags]
```

### Options

```
  -h, --help   help for db
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

* [./cells-enterprise config](./cells-enterprise-config)	 - Configuration manager
* [./cells-enterprise config db add](./cells-enterprise-config-db-add)	 - Add a database connection to the configuration
* [./cells-enterprise config db list](./cells-enterprise-config-db-list)	 - List all database connections
* [./cells-enterprise config db set](./cells-enterprise-config-db-set)	 - Assign a database connection to a service

###### Auto generated by Pydio Cells Enterprise Distribution v2.1.5 on 31-Aug-2020
