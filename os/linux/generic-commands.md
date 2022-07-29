# User Management
## Add login user
1. Add user

    adduser username

2. Add to user group

    usermod -aG sudo username
    
# Networks
## Check NAT PUblic IP

    dig +short myip.opendns.com @resolver1.opendns.com
