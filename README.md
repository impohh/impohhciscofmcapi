# Cisco Firepower REST API 

# Features version 0.0.1

- get_networkaddresses() is a function to get network object (Host, Network, Range, FQDN)
```sh
get_networkaddresses()
```

- get_networkgroups() is a function to get network group object (include network object each groups)
```sh
get_networkgroups()
```

- get_ports() is a function to get port object
```sh
get_ports()
```

- get_ports() is a function to get port group object (include port object each groups)
```sh
get_portgroups()
```
> You can select one function or also more fuctions in your python file.

## Installation

install packet impohhciscofmcapi

```sh
> pip install impohhciscofmcapi
```

### example code (example.py)
```sh
from impohhciscofmcapi import *

server = "https://xxx.xxx.xxx.xxx"
username = "username"
password = "password"

connect(server, username, password)

get_networkaddresses()
get_networkgroups()
get_ports()
get_portgroups()
```

### Output path file
the output file is your desktop path (.xlsx)

### Example output in excel file
| ID_Objects | Name | Type | Value | Description | Overridable | Status | 
| ------ | ------ | ------ | ------ | ------ | ------ | ------ |
| D4C93CE4-15EC-0ed3-0000-034359778547 | 10.0.10.10 | Host | 10.0.10.10 | Host Client A | False |  |
| D4C93CE4-15EC-0ed3-0000-034359778547 | 10.0.20.0_24 | Host | 10.0.20.0/24 | Network AAA | False |  |