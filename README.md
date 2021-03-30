# toc-tkg-app-example

## This repo is for use with a companion blog post at [Thinking Out Cloud Blog](https://thinkingoutcloud.org)

## Installation

You will need a running Kubernetes Cluster.

## Files Included Here

- metallb-config.yaml: This is taken straight from the MetalLB website. You will need to alter line 21 with your legitimate IP range.
- nginx-lb-deployment.yaml: This is also taken from MetalLB. This was the best example of a deployment for learning that I could find.

## Usage

Once MetalLB and Ingress is installed and the K8s Cluster is ready:

```bash
kubectl create namespace whizbangapp
kubectl create -f metallb-config.yaml
kubectl create -f nginx-lb-deployment.yaml
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
