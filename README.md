# ansible-burrow

An Ansible role for installing [Burrow](https://github.com/linkedin/Burrow).

### what is burrow?

Burrow is a monitoring companion for Apache Kafka that provides consumer lag checking as a service without the need for specifying thresholds. It monitors committed offsets for all consumers and calculates the status of those consumers on demand. An HTTP endpoint is provided to request status on demand, as well as provide other Kafka cluster information. There are also configurable notifiers that can send status out via email or HTTP calls to another service.

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
