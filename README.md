# lycophron.org

Updating nginx.conf
```bash
sudo cp nginx.conf /etc/nginx/sites-available/default 
sudo service nginx restart
journalctl -f -u nginx.service
```

To renew the certificates run:
```bash
sudo service nginx stop
sudo certbot renew
#sudo /home/ubuntu/.local/share/letsencrypt/bin/letsencrypt --no-self-upgrade renew -nvv --standalone
sudo service nginx start
```
