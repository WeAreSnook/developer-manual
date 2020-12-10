# Deploying to GOV PaaS

[GOV Platform as a Service (PaaS)](https://www.cloud.service.gov.uk/) is like Heroku for public sector projects. It allows public sector teams to host applications in a government approved cloud environment. It is built on top of the open source [Cloud Foundry](https://github.com/cloudfoundry) platform.

## Documentation

[The official Platform as a Service docs](https://docs.cloud.service.gov.uk/#gov-uk-platform-as-a-service) should always be your first port of call. This guide serves more as evolving checklist of helpful tips to help you get set up for success.

## Important questions to ask the client

- Will the system need to store data classified as higher than official? If yes: we can't use Gov PaaS.
- Do you already have a Gov PaaS account?
- Who manages your IT / infrastructure?
- Who should involve from an IT / Infrastructure?
- Who will be managing this service in production?
- What application monitoring tools do you use?
- What log monitoring tools do you use?

## Checklist

- [ ] **To set up a GOV PaaS account you need a `.gov.uk` email.** This email account will often be responsible for managing applications across an orgnanisation. If the organisation doesn't already have a GOV PaaS account, the infrastructure / IT team should be responsible for setting it up. If they do have an account, we will want to work closely with the team who manages it from as early as possible in the project.
- [ ] **Create a `manifest.yml` file in the root of your repository.** GOV PaaS uses a configuration file to provision and deploy your app.
