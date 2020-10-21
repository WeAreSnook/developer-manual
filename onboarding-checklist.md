# Onboarding checklist

We want to make it easy for new developers to join Snook. Whether people are just collaborating on one project or joining the team full-time, people should feel:

- **included**
- **involved**
- **ready**

We've put together this onboarding checklist for people responsible for onboarding a new team member. It is likely to be incomplete or out of date.

If you think of a way it could be improved, create an issue in the [Developer Manual](https://github.com/WeAreSnook/developer-manual) or even better suggest the change through a [pull request](pull-requests.md).

## When a developer joins Snook

### If they are a contractor

- [ ] **Add them to the [Github](https://github.com/WeAreSnook) project they are working on**. Associate and mid-level developers should be added as `members`. Senior and principal developers should be added as `owners`.
- [ ] **Add them to [Heroku](https://dashboard.heroku.com/teams/snook/access)**. Associate and mid-level developers should be added as `members`. Senior and principal developers should be added as `admin`.
- [ ] **Help them to login with Github to set up a [CircleCI](https://circleci.com/vcs-authorize/) account**. They will need to grant access to the WeAreSnook organisation on Github to see pipelines.
- [ ] Help them [setup their laptop](#laptop-setup)
- [ ] Talk to the ops team to give them access to relevant Slack channels.
- [ ] Give them a warm intro on Slack
- [ ] Add them to any important calendar invitations e.g. standups etc.

### If they are a permanent team member

Snook's Ops teams take care of new team members' company onboarding. This includes things like:

- setting up an email account
- adding them to Slack
- granting them file access
- orienting them in the company

Alongside their company onboarding, it's important that people have a clear onboarding to the team.

- [ ] **Add or invite them to the [wearesnook](https://github.com/orgs/WeAreSnook/people) Github organisation**. Associate and mid-level developers should be added as `members`. Senior and principal developers should be added as `owners`.
- [ ] **Add them to [Heroku](https://dashboard.heroku.com/teams/snook/access)**. Associate and mid-level developers should be added as `members`. Senior and principal developers should be added as `admin`.
- [ ] **Help them to login with Github to set up a [CircleCI](https://circleci.com/vcs-authorize/) account**. You will need to grant access to the WeAreSnook organisation on Github to see pipelines.
- [ ] Help them [setup their laptop](#laptop-setup)
- [ ] Invite them to any important calendar invitations e.g. standups, team calls etc.

## Laptop setup

These are some of the tools we install to set up our laptops for development.

- [ ] **[Git](https://git-scm.com/downloads)** - For version control
- [ ] **[Homebrew](https://brew.sh/)** - For managing packages on Mac OS
- [ ] **[Docker](https://www.docker.com/get-started)** - For creating repeatable development environments
- [ ] **[Postgres](https://www.postgresql.org/)** - For databases - install with Homebrew
- [ ] **[Redis](https://redis.io/)** - For key/value store, mainly used with Sidekiq for processing background jobs or as a Cache - install with Homebrew
- [ ] **[RVM](https://rvm.io/)** - Managing Ruby versions
- [ ] **[Rails 6](https://rubyonrails.org/)** - Our primary web framework
- [ ] **[NVM](https://github.com/nvm-sh/nvm)** - Managing Node versions
- [ ] **[Yarn](https://yarnpkg.com/)** - JavaScript dependency management. Rails is set up to use yarn.
- [ ] **[VSCode](https://code.visualstudio.com/)** - Text editing
- [ ] **[Postman](https://www.postman.com/)** - For documentation and testing of APIs and web services

Longer term, we want to automate set up of new laptops inspired by Thoughtbot's [laptop script](https://github.com/thoughtbot/laptop).

## VSCode Plugins

_Here we'll put required and recommended VSCode plugins_

## Background reading

We have put together a reading list to help people orient themselves in the team.

### Our principles

As a team we have three core principles that guide our daily actions:

#### 1.Universal access

— We design and build technology that everyone can use.
— We care deeply about accessibility and equality of access.

#### 2.Delightfully useful

— Our work is useful, usable and aligned to user goals.
— Beyond utility, we build things that bring delight into people's lives and help them thrive.

#### 3. Radically adaptive

— We respond quickly to people’s emerging needs and a world in flux.
— We choose tools and methods to design and build technology for change.

### How we work

- Our delivery process aligns closely with the GDS [Digital Service standard](https://www.gov.uk/service-manual/service-standard).
- We create software that conforms to the principles of [12 Factor Apps](https://12factor.net/).
- We align the team around the [values](https://www.agilealliance.org/agile101/the-agile-manifesto/) and [principles](https://www.agilealliance.org/agile101/12-principles-behind-the-agile-manifesto/) of the Agile manifesto over a tribe of Agile like Scrum or XP. There is also [a helpful video](https://www.youtube.com/watch?v=LMnozmayNJQ) that covers the 12 principles of Agile if you find that easier. **Learn more about our approach to [Agile](agile/)**.

### Technology

- [TDD](https://github.com/WeAreSnook/developer-manual/issues/9) - How we approach test driven development
- [Managing secrets](https://github.com/WeAreSnook/developer-manual/issues/10) - How we keep secrets....well secret 🗝
