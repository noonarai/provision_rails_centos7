## Getting Started

Set up an environment of RoR
(with centos7, apache, passenger, mariadb, rbenv)

```
$ git clone git@github.com:noonarai/provision_rails_centos7.git MYAPP
$ cd MYAPP
$ rm -rf .git .gitignore README.md
$ sed -i "" -e "s/MYAPP/my_sample_app/g" Vagrantfile  # change 'my_sample_app'
$ vagrant up
$ vagrant ssh
```

```
$ cd /home/vagrant/MYAPP
$ bundle install --path vendor/bundle
$ bundle exec rails new . -Bf -d mysql
```
