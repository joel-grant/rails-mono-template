This repo is a ready-to-go Ruby on Rails project with the following additional features:
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


