# AWS copy multiple ssh public keys to  ec2 intense
# Main playbook 
![](README/Screen%20Shot%202018-10-15%20at%201.33.30%20AM.png)


# Adding your list of public keys 
Please follow the steps to best results. 

 Open the `copy_public_kyes` playbook and change variable public_keys to your list.
``` 
     public_keys:
      - ssh-rsa 121
      - ssh-rsa 122
      - ssh-rsa 123
``` 

# Please change the hosts file to your remote hosts
![](README/Screen%20Shot%202018-10-15%20at%201.35.19%20AM.png)

# Run the playbook 
```
ansible-playbook -u centos  --private-key=keyforec2.pem copy_public_kyes.yml
```
![](README/Screen%20Shot%202018-10-15%20at%201.37.07%20AM.png)

# Try to login as root 
![](README/Screen%20Shot%202018-10-15%20at%201.39.45%20AM.png)


Thank you  for using my playbook😊 


