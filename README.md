1. Nodejs application Initialization: First, a basic Node.js application was created with index.js and a simple test file.

2.Locally testing the application: The application was tested locally to ensure the server and test script were functional.

3.Docker Integration: A Dockerfile and a .dockerignore file were added to the project to enable containerization.

4.Git and GitHub Setup: The project was initialized as a Git repository, linked to a new remote repository on GitHub, and the initial files were pushed.

5.For Workflow: The main.yml file was created to define the automated CI/CD pipeline, specifying the steps for GitHub Actions to follow.

6.Configuration and Debugging:

The workflow failed due to syntax errors in main.yml, which were resolved by correcting the indentation and formatting.

The pipeline failed again because a required package-lock.json file was missing, which was resolved by generating and pushing the file.

The workflow's authentication to Docker Hub failed because the required DOCKERHUB_USERNAME and DOCKERHUB_TOKEN secrets were not yet configured in the GitHub repository.

7.Successful Execution: After all configuration issues were resolved, the workflow ran successfully, confirming that the CI/CD pipeline was operational, building, and pushing the Docker image.
