# ansible

ansible
├── inventories
│   └── production
│       └── hosts
├── playbook.yml
└── roles
    ├── common
    │   ├── files
    │   │   └── index.html
    │   └── tasks
    │       └── main.yml
    └── nginx
        ├── handler
        │   └── main.yml
        ├── handlers
        │   └── main.yml
        ├── tasks
        │   └── main.yml
        └── templates
            └── nginx.conf.j2


1. Genrate a Public key on Control_machine using "ssh-keygen" command
   "ssh-keygen"

2. copy the ssh key id to target machine 
  "ssh-copy-id <your_username>@<target_machine>"

3. create a inventory file a paste the target machine IP Address
  "[web_servers]
   target_machine "

4. to check the connection to target machine 
   "ansible -i inventories/production/hosts -m ping"

5. Create roles for NGINX and COMMONS for HTML page

6. Create a Playbook and call ansible-playbook command
    "ansible-playbook -i inventories/production playbook.yml"

