This repo was created with: `rails new rails-mono-template -T -d=postgresql`
- run `rails g rspec:install`

It comes prepared with:
- RSpec
- Postgresql 17
- Additional gems
  - pry
  - rspec
  - vcr
  - webmock
  -

A new user of this template should:
- run `bundle install`
- run `rails db:create`
- run `VISUAL="code --wait" bin/rails credentials:edit`

A user of this repo should use the following tools for development:
- Docker Desktop/CLI
- Docker compose CLI
- GitHub CLI
- Kubectl
- Rubocop
- Ruby v3.4.3
- Rails v8.0.2
- Helm



### Some helpful Rails Commands:
`bin/rails generate model Article title:string body:text`
`rails db:migrate`
`rails console`

### Migrations
rails g migration CreateWatchItems entity_type:integer entity:integer user:references

Secrets to set up:
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

bin/rails credentials:edit

Create a workspace/repo in:
- Docker hub
- CloudSmith

Use this with a specific helm chart.
