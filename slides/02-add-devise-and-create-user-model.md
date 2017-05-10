*Add Devise and Create Users Model**

1. Add Devise Gem in `Gemfile`.
```ruby
gem 'devise', github: 'plataformatec/devise', ref: '83002017'
```

2. Install the dependencies.
```shell
bundle install
```

3. Run Devise Installation
```shell
rails generate devise:install
rails g devise:views
rails g devise User
rails db:migrate
```

4. Checking User Model
```ruby
rails c

> @users = User.all
  User Load (2.9ms)  SELECT  "users".* FROM "users" LIMIT ?  [["LIMIT", 11]]
 <ActiveRecord::Relation [#<User id: 1, email: "enogrob@gmail.com", created_at: "2017-05-06 09:34:52", updated_at: "2017-05-06 09:34:52">]>

> @users = User.all.count
   (5.6ms)  SELECT COUNT(*) FROM "users"
 => 1
>
```

5. Commit `add_user`
```shell
git status
git add .
git commit -am "add devise and create user model"
```
