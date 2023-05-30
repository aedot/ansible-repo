# ansible-repo

## Requirements

```
pip3 install -r requirements.txt
```

## Inventory

```
ansible-vault encrypt inventory.ini
ansible-vault decrypt inventory.ini
```

## Ansible Command

### Ping nodes
```
ansible all -m ping
```

### Run Playbook

```
ansible-playbook <playbook_directory>
```

### Encrypt file

```
ansible-vault encrypt <filename.extenstion>
```

### Encrypt ansible-vault string

```
ansible-vault encrypt_string '<password>' --name '<password_name>'
```

### Decrypt ansible-vault string

```
echo '<ansible vault string>' | tr -d ' ' | ansible-vault decrypt && echo
```
