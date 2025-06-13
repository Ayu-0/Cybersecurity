# Firewalls Tools & Configs (Linux):

## ufw :

- Install it using your package manager
- Now, there is config file located in /etc/default/ufw
- We'll edit them and make change acc to our need

But first what does ufw do?
- So as name suggest it's simple config tool to manage firewalls

So how we do configure it ?
- Edit using sudo nano /etc/default/ufw

OK there is basic guide to understand what to do :

1. Want to block incoming or outgoing connection, just run 
```
sudo ufw default deny incoming
```
```
sudo ufw default allow outgoing
```

2. Allow basic services :
- Allow SSH (important if using remote login)
```
sudo ufw allow ssh
```

- Or specify the port
```
sudo ufw allow 22
```

- Allow HTTP and HTTPS
```
sudo ufw allow http
sudo ufw allow https
```
- Allow specific app
```
sudo ufw allow 'OpenSSH'
```

- You can allow specific port and protocol
```
sudo ufw allow 53/udp       # DNS
sudo ufw allow 80/tcp       # HTTP
```

3. You can specify port ranges with UFW. Some applications use multiple ports, instead of a single port.
```
sudo ufw allow 6000:6007/tcp
sudo ufw allow 6000:6007/udp
```

4. Want to add specific ip address :
``` 
sudo ufw allow from 203.0.113.4
sudo ufw deny from 203.0.113.4
```


Sources for detailed guide -
1. https://www.digitalocean.com/community/tutorials/how-to-set-up-a-firewall-with-ufw-on-ubuntu
2. 