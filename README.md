# E-commerce Solidarity Economy

I need to warning you, it still a working in progress. So, if you need a complete one, it's not ready yet.

## Stack

- Rails 7.0.5
- Sqlite
- Devise Token Auth for authentication

## How to use it?

Basically we have some endpoints to be used by users with specifically permissions.

We have two profiles on app: `admin` and `client`.

**Admin** is the person responsible to manage everything. He can CRUD *Category*, *Product*, *Promotion* and *Payment*.\
**Client** is the profile permitted to make and order.\
And we also have **unauthenticated** routes as Product lists and searching.

## Building application

Ok, so first you must have:

1. Sqlite installed.

2. Ruby >= 2.5.0 installed (minimum required for Rails 6.0.3.3, version we're working with).

3. As we're on the beginning of project, don't forget to right configure your `datatabe.yml`.

4. And to *bundle* it with command:

```
bundle install
```
As soon as you have everything done you can follow


### 1. Task to build dev environment

```
rails dev:prime
```

### 2. Manually building everything

If you want to rock and create your dev environment and data, it's possible to go through the usual way

1. Create databases
```
rails db:create
```

2. Run migrations
```
rails db:migrate
```

3. Start the server
```
rails s
```

If you want to run tests:
```
bundle exec rspec
```

