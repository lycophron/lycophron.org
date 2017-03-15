# lycophron.org


To renew the certificates run:
```bash
sudo service nginx stop
sudo /home/ubuntu/.local/share/letsencrypt/bin/letsencrypt --no-self-upgrade renew -nvv --standalone
sudo service nginx start
```
