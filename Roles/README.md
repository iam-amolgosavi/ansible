# Create a role 

 ansible-galaxy role init httpd

 ls -ltr httpd

 cd httpd

 ls

 cd ../..

 ansible-playbook first-playbook.yml

 # tree Structure:
 
 ```
 <role_name>/
  ├── defaults/
  │   └── main.yml
  ├── files/
  ├── handlers/
  │   └── main.yml
  ├── meta/
  │   └── main.yml
  ├── tasks/
  │   └── main.yml
  ├── templates/
  ├── vars/
      └── main.yml
```
