## ./cec completion

Auto completion for Pydio Cells

### Synopsis

Completion for Pydio Cells Client
	 
	 # Add to current session
	 source <(cec completion bash)
	 # Add to current zsh session
	 source <(cec completion zsh)
	 
	 # Add bashcompletion file (might require sudo)
	 cec completion bash > /etc/bash_completion.d/cec
	 # Add zshcompletion file
	 cec	completion zsh > ~/.zsh/completion/_cec
	 

```
./cec completion [flags]
```

### Options

```
  -h, --help   help for completion
```

### Options inherited from parent commands

```
  -c, --config string   Path to the configuration file
```

### SEE ALSO

* [./cec](./cec)	 - Connect to a Cells Server using the command line
* [./cec completion bash](./cec-completion-bash)	 - 
* [./cec completion zsh](./cec-completion-zsh)	 - 

###### Auto generated by spf13/cobra on 31-Oct-2019