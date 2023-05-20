# cloudflare Access

## Install Cloudflare cli on client machine (cloudflared)
  https://developers.cloudflare.com/cloudflare-one/connections/connect-apps/install-and-setup/installation/
  
## Assuming you already installed and set up shh  
  ### open file ~/.ssh/config
     sudo nano ~/.ssh/config
  ### Add The following contents
      Host host.domain.com (your host url)
      ProxyCommand /usr/local/bin/cloudflared access ssh --hostname %h
  ### Proceed to ssh
      ```ssh username@domain```
      
 Congrats You made it !!!
  
