Move and/or rename nodes on the server

### Synopsis

Move and/or rename nodes on the server

```
./cec mv [flags]
```

### Examples

```

# Move a node
./cec mv common-files/formula-one.jpg personal-files/photos/

# Rename a node
./cec mv common-files/formula-one.jpg common-files/f1.jpg

# Move all nodes recursively 
./cec mv common-files/photos/* personal-files/photos/

```

### Options

```
  -h, --help   help for mv
```

### Options inherited from parent commands

```
  -c, --config string   Path to the configuration file
```

### SEE ALSO

* [./cec](./cec)	 - Connect to a Pydio Cells server using the command line

###### Auto generated by Cells Client v2.0.6 on 22-Jun-2020
