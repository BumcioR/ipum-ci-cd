# ipum-ci-cd

Deployment & CI/CD

This project focuses on the continuous integration (CI) and continous delivery (CD)
pipelines for deployment of ML models, as well as optimization of models for
inference after training. Those operations allow safe, automated and efficient
updates of models to production environment.

GitHub Actions for CI pipelines were used due to their simplicity and popularity.
For model compilation and optimization, ONNX tools were used to convert our models
to a versatile and efficient format.

Conditional execution has been implemented, enabling running of pipeline stages and integration.
AWS integration was achieved by configuring AWS credentials and Multi-Factor Authentication (MFA) has been included to enhance security.
Docker image building was included in the pipeline, the image was built, tagged and pushed to a private Amazon ECR repository.
This facilitates versioning and secure container storage.
