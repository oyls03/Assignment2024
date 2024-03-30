Run a simple Nginx ingress pod on EKS.

Provision the resources with Terraform
    terraform init
    terraform plan
    terraform apply

Then move on to deploy and adopt resources
    kubectl apply -f deployment.yaml

Then create the service
    kubectl apply -f service.yaml

Retrieve the external IP with
    kubectl get svc -A

Tear down everything
    terraform destroy
