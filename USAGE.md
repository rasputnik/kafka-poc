# client config

Once Ansible has run you have a 3 broker cluster
with one zookeeper. Most clients are going to want to
know their details.

If you used the hostmanager plugin, names should resolve fine.


# zookeeprs list

Consumers tend to use this. We have one, and the kafka config
is put under the /kafka znode, so you want

    zk1:2181/kafka

# broker list

Producers typically need this rather than just a zk URL.

    kafka1:9092,kafka2:9092,kafka3:9092

