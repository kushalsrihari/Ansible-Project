# ansible

my_nginx_ansible_project/
├── ansible.cfg
├── inventories/
│   └── production/
│       └── hosts
├── roles/
│   ├── common/
│   │   ├── tasks/
│   │   │   └── main.yml
│   │   └── files/
│   │       └── index.html
│   └── nginx/
│       ├── tasks/
│       │   └── main.yml
│       ├── handlers/
│       │   └── main.yml
│       └── templates/
│           └── index.html.j2
└── playbook.yml


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

