## jx-verify ingress

Verifies the ingress configuration defaulting the ingress domain if necessary

### Usage

```
jx-verify ingress
```

### Synopsis

Verifies the ingress configuration defaulting the ingress domain if necessary

### Examples

  # populate the ingress domain if not using a configured 'ingress.domain' setting
  jx step verify ingress

### Options

```
  -d, --dir string                 the directory to look for the values.yaml file (default ".")
      --external-ip string         The external IP used to access ingress endpoints from outside the Kubernetes cluster. For bare metal on premise clusters this is often the IP of the Kubernetes master. For cloud installations this is often the external IP of the ingress LoadBalancer.
  -h, --help                       help for ingress
      --ingress-namespace string   The namespace for the Ingress controller (default "kube-system")
      --ingress-service string     The name of the Ingress controller Service (default "jxing-nginx-ingress-controller")
      --lazy-create string         Specify true/false as to whether to lazily create missing resources. If not specified it is enabled if Terraform is not specified in the jx-requirements.yml file
  -n, --namespace string           the namespace to install into. Defaults to $DEPLOY_NAMESPACE if not
      --provider string            Cloud service providing the Kubernetes cluster.  Supported providers: aks, alibaba, aws, eks, gke, icp, iks, jx-infra, kubernetes, oke, openshift, pks
```

### Options inherited from parent commands

```
  -b, --batch-mode   Runs in batch mode without prompting for user input
      --verbose      Enables verbose output. The environment variable JX_LOG_LEVEL has precedence over this flag and allows setting the logging level to any value of: panic, fatal, error, warn, info, debug, trace
```

### SEE ALSO

* [jx-verify](jx-verify.md)	 - commands for verifying Jenkins X environments

###### Auto generated by spf13/cobra on 3-Jul-2020