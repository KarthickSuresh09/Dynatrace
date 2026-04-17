This command is the "installer" for the Dynatrace Operator, 
which is the management layer that automates the deployment and maintenance of monitoring in your cluster.

```
  helm install dynatrace-operator oci://public.ecr.aws/dynatrace/dynatrace-operator \
  --create-namespace \
  --namespace dynatrace \
  --rollback-on-failure
```
