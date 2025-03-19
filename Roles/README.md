# Create a role 

 ansible-galaxy role init httpd

 ls -ltr httpd

 cd httpd

 ls

 cd ../..

 ansible-playbook first-playbook.yml

 # tree Structure:
 
 
 ├── README.md
 
├── defaults
│   └── main.yml
├── files
│   └── index.html
├── handlers
│   └── main.yml
├── meta
│   └── main.yml
├── tasks
│   └── main.yml
├── templates
├── tests
│   ├── inventory
│   └── test.yml
└── vars
    └── main.yml
