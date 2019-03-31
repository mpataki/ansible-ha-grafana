# ansible-grafana

[![Build Status](https://travis-ci.org/mpataki/ansible-ha-grafana.svg?branch=master)](https://travis-ci.org/mpataki/ansible-ha-grafana)

[Grafana](https://grafana.com/) is a dashboard/metric visualization tool for time series data like that collected by home home assistant. This ansible role installs and configures grafana to pull data from [InfluxDB](https://www.influxdata.com/).

This can be installed via ansible galaxy or git.

## Requirements

Really this should work on any debian based system, but has been tested on a Raspberry Pi running Hassbian.

## Role Variables

None.

## Dependencies

- [ha-influxdb](https://github.com/mpataki/ansible-ha-influxd://github.com/mpataki/ansible-ha-influxdb)

## Example Playbook

```yml
    - hosts: pi
      roles:
         - role: mpataki.ha-grafana
```

## License

MIT
