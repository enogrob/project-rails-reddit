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
git commit -am "first commit"
hub create
```

4. Scaffold link.
```shell
git checkout -b link_scaffold
rails g scaffold link title url
rake db:migrate
```

5. Update git for link_scaffold
```shell
git status
git add .
git commit -am "performed generation links scaffold"
```

6. Merge with master.
```shell
git checkout master
git merge link_scaffold
git push origin master
```
