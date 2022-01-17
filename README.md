```
python3 -m venv venv
. ./venv/bin/activate
pip install -r requirements.txt
```

```
cp inventory.example inventory
```

Edit `inventory` with your server IP and User and change the vars with what you need.  
**Please also notice that you'll need to copy your offline file to your server manually in the path that you specify in the `offfi` variable.**

```
ansible-playbook -i inventory playbook.yml --ask-become-pass
```