# Ansible Vaults:
# Ansible Vault is a feature provided by Ansible that allows you to encrypt sensitive data within Ansible playbooks, roles, and other files.

```ansible-vault create test.yaml```  -> to create the file in encrypted format.

```ansible-vault decrypt test.yaml``` -> to decrypt the file

```ansible-vault edit test.yaml``` -> This command will decrypt the file to a temporary file and allow you to edit the file

```ansible-vault rekey test.yaml``` -> to change the password.

```ansible-vault encrypt test.yaml``` -> to encrypt the existing file

```ansible-vault view test.yaml``` -> to view encrypted file.

```ansible-playbook new.yaml --check --ask-vault-pass ```-> you can run the encrypted playbbok

# vault-id:
```ansible-vault encrypt --vault-id database_pass@prompt database.yaml```

# ansible vault with password file.
```openssl rand -base64 24 | tee vault_pass.txt``` -> to create the random password

```ansible-vault encrypt --vault-id /etc/ansible/vault_pass.txt password.yaml``` -> encrypt the yaml file with the password file

```ansible-playbook password.yaml --vault-password-file /etc/ansible/vault_pass.txt``` ->run the yaml file

```ansible-vault decrypt --vault-id /etc/ansible/vault_pass.txt password.yaml``` -> decrypt the yaml file
