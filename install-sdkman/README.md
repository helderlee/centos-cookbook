```bash
sudo su
yum -y remove java*
export SDKMAN_DIR="/usr/local/sdkman" && curl -s "https://get.sdkman.io" | bash
chmod -R 777 /usr/local/sdkman/var
```

Edit file /home/user/.bashrc at the end:

```bash
#THIS MUST BE AT THE END OF THE FILE FOR SDKMAN TO WORK!!!
export SDKMAN_DIR="/usr/local/sdkman"
[[ -s "$SDKMAN_DIR/bin/sdkman-init.sh" ]] && source "$SDKMAN_DIR/bin/sdkman-init.sh"
```

Close and open the terminal.