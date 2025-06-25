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

A user of this repo should use the following tools for development:
- Docker Desktop/CLI
- Docker compose CLI
- GitHub CLI
- Kubectl
- Rubocop
- Ruby v3.4.3
- Rails v8.0.2



### Some helpful Rails Commands:
`bin/rails generate model Article title:string body:text`
`rails db:migrate`
`rails console`

### Migrations
rails g migration CreateWatchItems entity_type:integer entity:integer user:references