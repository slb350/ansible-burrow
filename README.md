# ansible-burrow

An Ansible role for installing [Burrow](https://github.com/linkedin/Burrow).

## Role Variables

- `GOPATH` - your go env path
- `sudo_user` - user who's go env you are using
- `sudo_group` - group for your go user
- `burrow_link` - link to linkedin's burrow (default: `github.com/linkedin/burrow`)
- `logdir` - directory you wish to log to (default: `/var/log`)
- `zookeeper_host` - zookeeper hostname(s) or ip(s)
- `zookeeper_port` - zookeeper port (default: `2181`)
- `kafka_cluster_name` - kafka cluster name
- `kafka_broker_host` - kafka hostname(s) or ip(s)
- `kafka_port` - kafka port (default: `9092`)
