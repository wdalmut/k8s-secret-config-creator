# K8S secret configurations generator

Just a simple tool that merge temporary AWS credentials in a K8S Secret
configuration file


```
./config-creator update -s <development-cloudformation-stack-name>
```

Just check the `aws.yaml` file

## Custom command options

Run it with help

```
./config-creator update -s test --help

Usage: config-creator [options]

Options:
  -c, --credentials <filepath>   AWS Credentials (default: "/home/ash/.aws/credentials")
  -p, --profile <profile>        AWS Profile (default: "default")
  -r, --region <region>          AWS Region (default: "eu-west-1")
  -o, --output <path>            Save aws.yaml file at give path (default: "aws.yaml")
  -S, --silent                   expose created configuration in output (default: false)
  -s, --stack-name <stack-name>  Cloud Formation Stack Name
  -h, --help                     output usage information
```

