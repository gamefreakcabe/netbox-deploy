# netbox-deploy

Need to run create super user after playbook completes
```
source /opt/netbox/venv/bin/activate
```
```
source /opt/netbox/venv/bin/activate
cd /opt/netbox/netbox
python3 manage.py createsuperuser
```
Need these in variable for Ansible
- server_user
- db_password
- NEWVER (for both deploy and upgrade)
- OLDVER (for upgrade only)
- secret_key
- config_url (add account)
- county_code
- state_code
- locality
- org
- org_unit
- common_name
```
{
  "server_user": "",
  "db_name": "netbox",
  "db_user": "netbox",
  "db_password": "",
  "NEWVER": "",
  "OLDVER": ""
  "secret_key": "",
  "config_url": "https://raw.githubusercontent.com/<account>/netbox-deploy/main/configuration.py",
  "county_code": "US",
  "state_code": "GA",
  "locality": "Chicago",
  "org": "Company",
  "org_unit": "DevOps",
  "common_name": "netbox.name.org",
}
```
