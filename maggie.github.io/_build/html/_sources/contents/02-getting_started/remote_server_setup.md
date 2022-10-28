# Remote Server Setup & Access

The remote database is hosted on an Amazon EC2 server running on PostgreSQL. This server can only be accessed via whitelisted IP due to security reasons.  

<hr>

## Requesting EC2 Server Access

If you do not have permissions to access the server and need to access it for any reason, contact Xue with your local IPv4.

## Accessing the EC2 Server

Once your IPv4 has been whitelisted, enter the following command into the terminal to `ssh` into the server:  
```
ssh ec2-user@ec2-3-80-207-47.compute-1.amazonaws.com
```
    
To access the Django admin site with the remote database, enter the following into the EC2 server:  
```
screen -x
```

then navigate to the following url in a new browser window or tab:  
```
ec2-user@ec2-3-80-207-47.compute-1.amazonaws.com:8000/admin/
```