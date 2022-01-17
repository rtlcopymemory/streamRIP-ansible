```
python3 -m venv venv
. ./venv/bin/activate
pip install -r requirements.txt
```

```
cp inventory.example inventory
```

Edit `inventory` with your server IP and User

```
ansible-playbook -i inventory playbook.yml --ask-become-pass
```