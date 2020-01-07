## Exabgp role
[![Build Status](https://travis-ci.org/hybridadmin/ansible-role-exabgp.svg?branch=master)](https://travis-ci.org/hybridadmin/ansible-role-exabgp)

This role uses https://github.com/Exa-Networks/exabgp

#### Variables

##### General

* `bgp_neighbors`: [optional]: List of bgp neighbors to advertise prefixes to
* `community_list`: [optional]: communities to be used when advertising prefixes
* `anycast_cidrs`: [optional]: list of anycast cidrs to be advertised via bgp

#### Example

##### Basic example

```yaml 
bgp_neighbors:
  - ip: 10.220.50.10
    desc: "cr2"
    
community_list: "65359:500 65359:5000"

anycast_cidrs:
  - 10.220.59.188/32
  - 10.220.59.189/32
```

#### Author Information

Tinashe Chikomo
