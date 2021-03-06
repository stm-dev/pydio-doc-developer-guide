## ./cells doc i18n count

Count all Strings that are internationalised in the Pydio Cells code.

### Synopsis

Count all Strings that are internationalised in the Pydio Cells code.

Internationalised Strings are referenced in Pydio Cells code via Map[string]string in vanilla json files.
There are 3 types of Strings that are internationalised:

In Go code:
- Json files are nested in the various packages in lang/box subfolders and are used via github.com/nicksnyder/go-i18n library

In Javascript code (for the front):
- For the EndUser UI in ReactJS, json files are nested in the i18n subfolder and used via the MessageHash mechanism
- Strings that reside within the manifest.xml, are used on the back end side and are to be translated before being 
sent to the front end resides in the i18n/conf sub folder.

### Example

Use the --project-paths/-p flag to give path to at least one project root folder.

$./cells i18n count -p $GOPATH/src/github.com/pydio/cells-enterprise -p $GOPATH/src/github.com/pydio/cells


```
./cells doc i18n count [flags]
```

### Options

```
  -c, --convert-js                  Convert legacy JS files to new standard goi18n format
  -h, --help                        help for count
  -p, --project-paths stringArray   Root path of the project to analyse
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

* [./cells doc i18n](./cells-doc-i18n)	 - Internationalisation Utils

###### Auto generated by Pydio Cells Home Edition v2.1.5 on 31-Aug-2020
