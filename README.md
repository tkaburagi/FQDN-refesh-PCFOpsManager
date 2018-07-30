# FQDN-refesh-PCFOpsManager

This is a mitigation when it happens

`Invalid redirect https://FQDN/auth/cloudfoundry/callback did not match one of the registered values`


```bash
$ sudo -u postgres psql -d tempest_production -c "SELECT id, hostname from uaa_configs"

$ sudo -u postgres psql -d tempest_production -c "UPDATE uaa_configs set hostname='opsmanager.pcflab.jp' where id=1"

$ sudo -u postgres psql -d tempest_production -c "SELECT id, hostname from uaa_configs"

$ sudo shutdown -r now
```