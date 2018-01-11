### Dorado_Grafana
A templated Grafana dashboard for the Huawei Dorado all flash storage

Dependencies InfluxDB as the time-series database and Telegraf as the collector needs to be installed

For all latest files, see [My GitHub page](https://github.com/dkruyt/OceanStor_Grafana)

### Quick Start

* Enable SNMP on your Huawei Dorado storage
* Put dorado.conf in your `/etc/telegraf/telegraf.d` directory
* Edit the community string as appropriate
* Edit the SNMP verion as appropriate, please note that verion 2 is disabled by default on the Huawei OceanStor, check with `show snmp version` on the Storage
* Edit the 'agents' list to include all of your monitored Dorado storages
* Put the files in the mibs dir `/usr/share/snmp/mibs`
* Import the Grafana dashboard

### Screenshot

After you setup all, you should have some dashboard like this

![Grafana screenshot Dorado](https://github.com/dkruyt/Dorado_Grafana/blob/master/Huawei_Dorado_Storage.jpg?raw=true)
