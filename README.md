## MapR Ansible Modules

## export ansible library path
export ANSIBLE_LIBRARY=\`pwd\`

## list of modules
* mapr_service
```
To manage mapr services using rest api.
```

### examples
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

