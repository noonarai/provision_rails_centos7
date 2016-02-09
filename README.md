## Getting Started

Set up an environment of RoR
(with centos7, apache, passenger, mariadb, rbenv)

```
$ git clone git@github.com:noonarai/provision_rails_centos7.git MYAPP
$ cd MYAPP
$ find Vagrantfile provision_vagrant.sh | xargs sed -i "" -e "s/MYAPP/your_app_name/g"
$ vagrant up
```
