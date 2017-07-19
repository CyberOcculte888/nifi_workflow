# nifi_workflow
Nifi workflow

- [INSTALLATION](#installation)
- [CONFIGURATION](#configuration)
- [OPTIONS](#options)
- [LOG](#log)

# INSTALLATION

To install it right away for all UNIX users (Linux, OS X, etc.), type:

    sudo apt-get install netdata

To install netdata for CentOs/RHEL 5/6(not in repo):

    yum install netdata

To install python3 for CentOs/RHEL 7):

    yum install epel
    yum install netdata

# CONFIGURATION

Setting up configuration files :

    Update the configuration file /etc/netdata/netdata.conf with the below content:
    [backend]
	  enabled = yes
	  data source = average
	  type = json
	  destination = localhost:12100
	  # prefix = netdata
	  # hostname = 
	  update every = 15
	  buffer on failures = 10
	  timeout ms = 20000


Restart netdata service
    
    
# OPTIONS

    https://github.com/firehol/netdata/wiki/netdata-backends
    
# NIFI

Import Netdata.xml workflow into a nifi process group
