# Deploying a pytorch custom container to AWS Sagemaker using terraform

Checkout the video for a step by step guide here https://youtu.be/KFqehCAMaLQ !

1. Train the model using `main.py`
2. Test the endpoint locally using `uvicorn app:app --reload` command and send request using Postman.
3. Create a docker image using `Dockerfile` and push to ECR.
4. Use `terraform init`, `terraform plan` and `terraform apply --auto-approve` to deploy the model to AWS Sagemaker.
5. Test the endpoint using the AWS Sagemaker endpoint and `tests/test_endpoint.py` script.
6. Use `terraform destroy` to delete resources.