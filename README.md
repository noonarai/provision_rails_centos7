## Getting Started

Set up an environment of RoR
(with centos7, apache, passenger, mariadb, rbenv)

```
$ git clone git@github.com:noonarai/provision_rails_centos7.git MYAPP
$ cd MYAPP
$ find Vagrantfile provision_vagrant.sh | xargs sed -i "" -e "s/MYAPP/your_app_name/g"
$ vagrant up
```

※共有ディレクトリがマウントできないとかいうエラーが出た場合は、VitualBox GuestAdditionを入れ直す。
ホストOSのVagrantfileがあるディレクトリで
$ vagrant plugin install vagrant-vbguest
を実行してから vagrant up し直す。
