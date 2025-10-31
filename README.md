Note: This is a work in progress.  I've been toying with the concept of what it means to set up a new service effectively.  Adding new services to a distributed architecture can consume a lot of time and is prone to missed steps, missing documentation, and mistakes in configuration.  This repo has started as a playground to create an efficient way to create (for now) Rails 8 Applications that can be easily generated, configured, and deployed in a a repeatable way using autonation.  If a developer needs to create a new service for their application, what could takes hours could potentially take minutes.  Visitors are welcome to look around while I create something that accomplishes these goals effectively. 

### Included Features:
  - Additional gems
  - Postgresql
  - CI/CD Pipelines
    - Automated versioning and Changelogs, through "Conventional Commits"
    - Dependency vulnerabilities
    - Linting and Testing
    - Continuous Deployment to Kubernetes
  - Docker Compose ready
  - Other miscellaneous custom Rails configurations. 

This was originally generated with: 
- `rails new rails-mono-template -T -d=postgresql`
- `rails g rspec:install`

## Dependencies
- Ruby v3.4.3
- Rails v8.0.2
- Docker Desktop/CLI
- docker compose
- gh CLI
- Kubectl
- Rubocop
- Helm
---

## How to Use:
A new user of this template should:
- run `bundle install`
- run `rails db:create`
- run `VISUAL="code --wait" bin/rails credentials:edit`

The following secrets must be saved as GitHub Action Secrets in order to use all features:

DOCKERHUB_REPOSITORY
DOCKERHUB_TOKEN
DOCKERHUB_USERNAME
MY_RELEASE_PLEASE_TOKEN (This is a Github token)
KUBECONFIG
CLOUDSMITH_USER_NAME
CLOUDSMITH_API_KEY
DigitalOcean
  - POSTGRES_HOST
  - POSTGRES_USER
  - POSTGRES_PASSWORD
  - HELM_CHART
  - POSTGRES_DB
  - POSTGRES_PORT
  - RAILS_MASTER_KEY
  - RAILS_ENV
SECRET_NAME (name of the k8s generic secret you create)
release
HELM_CHART

### Create a workspace/repo in:
- Docker hub

### Some helpful Rails Commands:
`bin/rails generate model Article title:string body:text`
`rails db:migrate`
`rails console`

### Migrations
rails g migration CreateWatchItems entity_type:integer entity:integer user:references


