** Rails Reddit App**

1. Check versions.
```shell
rvm current

#=> ruby-2.1.1@rails-4.1.5
```

2. Create the Rails App, move into the app and test the server.
```shell
rails new rails-reddit-app

cd rails-reddit-app
rails s

```

3. Initialize `git`.
```shell
git init
git status
git add .
git commit -am "first-commit"
hub create
```

4. Scaffold link.
```shell
git checkout -b link_scaffold
rails g scaffold link title url
rake db:migrate
```

5. Set root address in `config/routes.rb` to:
```ruby
root 'links#index'
```

6. Commit git for `added-link-scaffolding`
```shell
git status
git add .
git commit -am "added-link-scaffolding"
```

6. Merge with master with `added-link-scaffolding`.
```shell
git checkout master
git merge added-link-scaffolding
git create
git push origin master
```
