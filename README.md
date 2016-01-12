## Getting Started

Set up an environment of RoR
(with centos7, apache, passenger, mariadb, rbenv)

```
$ git clone git@github.com:noonarai/provision_rails_centos7.git MYAPP
$ cd MYAPP
$ rm -rf .git .gitignore README.md
$ vagrant up
$ vagrant ssh
$ cd /vagrant
$ bundle install --path vendor/bundle
$ bundle exec rails new . -Bf -d mysql
```
