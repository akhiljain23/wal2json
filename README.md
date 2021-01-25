# Configure Wal2json

1. Create Schematics workspace using template https://github.com/Cloud-Schematics/VSI-database
2. Run Ansible command
```
ansible-playbook wal2json.yml -e "region=eu-gb deployment_id=<deployment-id> repl_password=<REPL_PASSWORD> slot_name=<SLOT_NAME> database_name=<DATABASE_NAME> bearer_token=<BEARER TOKEN>"
```

Sample Command:
```
ansible-playbook wal2json.yml -e "region=eu-gb deployment_id='crn:v1:bluemix:public:databases-for-postgresql:eu-gb:a/111111111111111111111111:22222222-2222-2222-2222-2222222222::' repl_password=Abc1234abc slot_name=myhappyslot database_name=ibmclouddb bearer_token='Bearer 11hgdvhgdvchgevdckjvedcjkvedcv'" -vvvv
```