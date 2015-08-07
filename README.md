kafka cluster on centos 6.

* single zookeeper on 'zk1'
* brokers running a kafka cluster

tested on OSX host.

# install

    vagrant plugin hostmanager install

    ansible-playbook -i vagrant/ site.yml

Then see **USAGE.md**.
