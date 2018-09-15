## MapR Ansible Modules

## export ansible library path
export ANSIBLE_LIBRARY=\`pwd\`

## list of modules
* mapr_service
* mapr_blacklistuser
```
To manage mapr services using rest api.
```

### examples for mapr_service
```
- mapr_service:
    username: mapr
    password: mapr
    service_name: nfs
    mcs_url: demo.mapr.com
    mcs_port: 8443
    state: restart
    validate_certs: false
```

### examples for mapr_blacklistuser
```
- mapr_blacklistuser:
    username: mapr
    password: mapr
    mcs_url: demo.mapr.com
    mcs_port: 8443
    validate_certs: false
    list_user: true

- mapr_blacklistuser:
    username: mapr
    password: mapr
    mcs_url: demo.mapr.com
    mcs_port: 8443
    validate_certs: false
    user: test
```