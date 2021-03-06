## ./cells-enterprise acl create

Create an Access Control

### Synopsis

Create an Access Control in the dedicated micro service

Use this command to manually grant a permission on a given node for a given role.


```
./cells-enterprise acl create [flags]
```

### Options

```
  -a, --action string         Action
  -v, --actionVal string      Action value
  -h, --help                  help for create
  -n, --node_id string        NodeIDs
  -r, --role_id string        RoleIDs
  -w, --workspace_id string   WorkspaceIDs
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

* [./cells-enterprise acl](./cells-enterprise-acl)	 - Manage access control lists

###### Auto generated by Pydio Cells Enterprise Distribution v2.1.5 on 31-Aug-2020
