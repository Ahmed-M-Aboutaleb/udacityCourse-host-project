# Hosting a Full-Stack Application

### **You can use you own project completed in previous courses or use the provided Udagram app for completing this final project.**

---

In this project you will learn how to take a newly developed Full-Stack application built for a retailer and deploy it to a cloud service provider so that it is available to customers. You will use the aws console to start and configure the services the application needs such as a database to store product information and a web server allowing the site to be discovered by potential customers. You will modify your package.json scripts and replace hard coded secrets with environment variables in your code.

After the initial setup, you will learn to interact with the services you started on aws and will deploy manually the application a first time to it. As you get more familiar with the services and interact with them through a CLI, you will gradually understand all the moving parts.

You will then register for a free account on CircleCi and connect your Github account to it. Based on the manual steps used to deploy the app, you will write a config.yml file that will make the process reproducible in CircleCi. You will set up the process to be executed automatically based when code is pushed on the main Github branch.

The project will also include writing documentation and runbooks covering the operations of the deployment process. Those runbooks will serve as a way to communicate with future developers and anybody involved in diagnosing outages of the Full-Stack application.

# Udagram

This application is provided to you as an alternative starter project if you do not wish to host your own code done in the previous courses of this nanodegree. The udagram application is a fairly simple application that includes all the major components of a Full-Stack web application.

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

### Installation

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres.
1. In AWS, provision a s3 bucket for hosting the uploaded files.
1. In AWS, provision a Elastic Beanstalk App.
1. Add the Env Vars to your environment variables.
1. Run npm run api:install && npm run frontend:install to install the dependencies.
1. Run npm run api:build && npm run frontend:build to build the applications.
1. Run npm run api:start && npm run frontend:start to start the applications.

## Api Endpoints

-   Front-End: http://projectudacity000.s3-website-us-east-1.amazonaws.com/
-   Back-End: http://app-env.eba-nrdmu7dv.us-east-1.elasticbeanstalk.com/

## Env Vars

-   POSTGRES_HOST ( DB link )
-   POSTGRES_USER ( DB user )
-   POSTGRES_PASSWORD ( DB password )
-   POSTGRES_DB ( DB name )
-   AWS_REGION ( AWS region )
-   URL ( Front-End Url )
-   JWT_SECRET ( JWT secret )
-   EB_APP ( EB app name )
-   EB_ENV ( EB env name )
-   AWS_BUCKET ( S3 bucket name )
-   AWS_ACCESS_KEY_ID ( AWS access key id )
-   AWS_SECRET_ACCESS_KEY ( AWS secret access key )

## Circle Ci

![Alt text](https://github.com/Ahmed-M-Aboutaleb/udacityCourse-host-project-/blob/main/docs/3.png 'CircleCi')

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

-   [Angular](https://angular.io/) - Single Page Application Framework
-   [Node](https://nodejs.org) - Javascript Runtime
-   [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
