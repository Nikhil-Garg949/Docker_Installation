**If we run a code and give that type of error:**
 ansible-playbook docker_installation.yml

PLAY [Create a kubernetes Cluster] *************************************************************************************************************************

TASK [Gathering Facts] *************************************************************************************************************************************
fatal: [localhost]: UNREACHABLE! => {"changed": false, "msg": "Failed to connect to the host via ssh: @@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@\r\n@         WARNING: UNPROTECTED PRIVATE KEY FILE!          @\r\n@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@\r\nPermissions 0644 for '/root/Docker_Installation/private_key.pem' are too open.\r\nIt is required that your private key files are NOT accessible by others.\r\nThis private key will be ignored.\r\nLoad key \"/root/Docker_Installation/private_key.pem\": bad permissions\r\nec2-user@localhost: Permission denied (publickey,gssapi-keyex,gssapi-with-mic).", "unreachable": true}

PLAY RECAP *************************************************************************************************************************************************
localhost                  : ok=0    changed=0    unreachable=1    failed=0    skipped=0    rescued=0    ignored=0

**Note:- If give that type of error so change the permission of Private Key**
**{chmod 400 private_key.pem}**

**Also give Your private key in this private_key.pem file**
