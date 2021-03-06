Configure a connection to a running server and locally persist credentials for later use

### Synopsis


Launch an interactive process to configure a connection to a running Pydio Cells server instance.
By default, we use a secure OAuth2 process based on 'Authorization Code' Grant.

If necessary, you might use an alternative authorization process and/or execute this process non-interactively calling one of the defined sub-commands.

Once a connection with the server established, it stores necessary information locally, keeping the sensitive bits encrypted in the local machine keyring.
If you want to forget a connection, the config file can be wiped out by calling the 'clear' subcommand.

*WARNING*
If no keyring is defined in the local machine, all information is stored in *clear text* in a config file of the Cells Client working directory.
In such case, do not use the 'client-auth' process.


```
./cec configure [flags]
```

### Options

```
  -h, --help         help for configure
      --no-keyring   Explicitly tell the tool to *NOT* try to use a keyring. Only use this flag if you really know what your are doing: some sensitive information will end up stored on your file system in clear text.
```

### Options inherited from parent commands

```
  -c, --config string   Path to the configuration file
```

### SEE ALSO

* [./cec](./cec)	 - Connect to a Pydio Cells server using the command line
* [./cec configure client-auth](./cec-configure-client-auth)	 - Connect to the server directly using the Client Credentials
* [./cec configure oauth](./cec-configure-oauth)	 - User OAuth2 to login to server

###### Auto generated by Cells Client v2.0.6 on 22-Jun-2020
