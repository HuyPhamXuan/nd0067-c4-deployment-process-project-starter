The application consists of a backend and a frontend.

For the backend, you will need an API that interacts with the database.

Database: You can use AWS RDS to host your database.
API: Deploy the API to the cloud using Elastic Beanstalk.
For the frontend, the files generated after building will be deployed as a static website.

Use S3 to host the frontend.
The frontend on S3 will interact with the API on Elastic Beanstalk, which in turn will communicate with the RDS database.