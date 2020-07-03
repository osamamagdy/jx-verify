## jx-verify dns

Verifies DNS resolution for ingress rules

### Usage

```
jx-verify dns
```

### Synopsis

This step checks that dns has propagated for all ingresses

### Examples

  jx step verify dns --timeout 10m

### Options

```
  -h, --help               help for dns
  -t, --timeout duration   The default timeout for the endpoint to return the expected HTTP code (default 10m0s)
```

### Options inherited from parent commands

```
  -b, --batch-mode   Runs in batch mode without prompting for user input
      --verbose      Enables verbose output. The environment variable JX_LOG_LEVEL has precedence over this flag and allows setting the logging level to any value of: panic, fatal, error, warn, info, debug, trace
```

### SEE ALSO

* [jx-verify](jx-verify.md)	 - commands for verifying Jenkins X environments

###### Auto generated by spf13/cobra on 3-Jul-2020