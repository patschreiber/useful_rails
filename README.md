# useful_rails
 A general list and cheatsheet of useful Rails programming structures and "gotchas."

## Managing Ruby versions
Use RVM to run different versions of Ruby. Use RVM's gemsets to create packages of gems. This is useful if you have multiple Rails projects and don't want to intermingle gems from different projects
### RVM
##### Install a ruby version
`rvm install 2.2.7`
##### Create a gemset
`rvm gemset create gemset_name`
##### Use specific ruby version and gemset
`rvm use 2.2.7@gemset_name`

### Rake
##### View all routes
`$ rake routes`
##### Runs database setup and migrations. This is run when the database is first set up, or if it doesn't exist
`$ rake db:setup`
##### Runs database migrations
`$ rake db:migrate`
##### Runs database seeds
`$ rake db:seed`

### Rails cli
##### Install Rails bundled gems
`bundle install`
##### Start Rails server
`$rails s`
##### Start Rails console
`$ rails c`

### Rails helpers
##### Gets the whole URI (e.g. https://localhost:3000/sign-up)
`<%= request.url %>`
##### Gets just the path (e.g. /sign-up)
`<%= request.path %>`