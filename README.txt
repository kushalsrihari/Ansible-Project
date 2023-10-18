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
│   └── nginx/
│       ├── tasks/
│       │   └── main.yml
│       └── templates/
│           └── index.html.j2
└── playbook.yml
