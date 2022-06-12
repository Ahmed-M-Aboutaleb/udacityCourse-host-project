## App Architecture

1. Client trying to access the website.
1. S3 bucket return the index.html file.
1. Client trying to access feature need the API.
1. S3 bucket send request to the API in Elastic beanstalk.
1. API get the data from AWS RDS.

![Alt text](https://github.com/Ahmed-M-Aboutaleb/udacityCourse-host-project-/blob/main/docs/2.png 'CircleCi PipeLine')
