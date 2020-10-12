# Heroku

We use [Heroku](https://heroku.com) for our hosting infrastructure, unless our project has specific infrastructure requirements.

## Why do we use Heroku?

- **Independence** - It allows any developer to quickly and easily build and deploy to production grade infrastructure.
- **Integration** - It plays well with our other tools like Github and CircleCI.
- **Speed** - We can get things online in a matter of minutes than days or weeks wrestling custom provisioning and deployment scripts.

## When we might not use Heroku?

- The project needs to be deployed on premises.
- The client wants it hosted on their infrastructure e.g. AWS, Google Cloud Platform.
- There are certain security requirements that can't be met by Heroku.
- We need to use backing services that can't be provisioned affordably within Heroku.

## Heroku pipelines

Heroku features the concept of [pipelines](https://devcenter.heroku.com/articles/pipelines).

> A pipeline is a group of Heroku apps that share the same codebase. Each app in a pipeline represents one of the following stages in a continuous delivery workflow.

All projects should minimally have the following environments configured:

- Review apps
- Staging
- Production

### Review apps

### Staging

### Production
