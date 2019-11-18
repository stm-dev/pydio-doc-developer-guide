## ./cells-enterprise install

Install Cells using a friendly user interface (browser)

### Synopsis

This command launch the installation process of Pydio Cells.

 It will ask for the Bind Host to hook the webserver on a network interface IP, and you can set different hosts for accessing
 the machine from outside world (if it is behind a proxy or inside a container with ports mapping for instance).
 
 You can launch this installer in non-interactive mode by providing --bind and --external. This will launch the browser-based
 installer, by default in self-signed mode. See the possible flags for more details.
 
 You can also use Let's Encrypt automatic certificate generation by providing a contact email and accepting Let's Encrypt EULA, for instance:
 $ ./cells-enterprise install --bind share.mydomain.tld:443 --external https://share.mydomain.tld --le_email admin@mydomain.tld --le_agree true

 For instance:
 - Bind Host: 0.0.0.0:8080
 - External Host: https://share.mydomain.tld
 Or
 - Bind Host: share.mydomain.tld
 - External Host: https://share.mydomain.tld
 Or
 - Bind Host: IP:1515       # internal port
 - External Host: https://IP:8080   # external port mapped by docker
 Or
 - Bind Host: IP:8080
 - External Host: https://IP:8080
 Or
 - Bind Host: localhost:8080
 - External Host: http://localhost:8080  # for non-secured local installation

 It will open a browser to gather necessary information and configuration for Pydio Cells. 
 Services will all start automatically after the install process is finished.
 
 If you do not have a browser access, you can also perform the whole installation process using this CLI.

 

```
./cells-enterprise install [flags]
```

### Options

```
      --bind string            Internal URL:PORT on which the main proxy will bind. Self-signed SSL will be used by default
      --external string        External PROTOCOL:URL:PORT exposed to the outside
  -h, --help                   help for install
      --json string            Points toward a configuration in JSON format
      --le_agree               Accept Let's Encrypt EULA
      --le_email string        Contact e-mail for Let's Encrypt provided certificate
      --le_staging             Rather use staging CA entry point
      --no_tls                 Generate locally trusted certificate with mkcert
      --tls_cert_file string   TLS cert file path
      --tls_key_file string    TLS key file path
      --yaml string            Points toward a configuration in YAML format
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

* [./cells-enterprise](./cells-enterprise)	 - Secure File Sharing for business

###### Auto generated by Pydio Cells Enterprise Distribution v2.0.0 on 5-Nov-2019