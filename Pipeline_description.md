The pipeline consists of 3 stages:

Build:

Install dependencies for the Frontend.
Install dependencies for the Backend.
Perform lint checks for the Frontend.
Build the Frontend.
Build the Backend. If the Build stage is successful, move to the Hold stage.
Hold:

Wait for manual approval from the user. If the user approves, proceed to the Deploy stage.
Deploy:

Install and build both the Backend and Frontend.
Sync the Frontend build folder to S3 for Frontend deployment.
Deploy the Archive.zip file, which is generated after building the Backend, to Elastic Beanstalk.
This pipeline ensures that both the Frontend and Backend are built and deployed automatically in your CI/CD process.