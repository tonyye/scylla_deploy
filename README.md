# scylla_deploy
```
sudo yum localinstall repo/createrepo-0.9.9-28.el7.noarch.rpm -y
createrepo --database /home/vagrant/repo
sudo yum-config-manager --add-repo file:///home/vagrant/repo
sudo yum --disablerepo=* --enablerepo=home_vagrant_repo install epel-release -y
sudo yum --disablerepo=* --enablerepo=home_vagrant_repo install scylla -y --nogpgcheck
```
