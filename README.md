# plugin-uplink

playSMS gateway plugin using other playSMS webservices to submit SMS

Info          | Value
------------- | ---------------------------------
Author        | Anton Raharja `<araharja@pm.me>`
Update        | 241119
Version       | 1.0
Compatible    | playSMS 1.4.7
playSMS       | https://playsms.org

# License

[MIT License](LICENSE)

# Installation

You will need an installed and working playSMS, preferred playSMS version 1.4.7 (current latest).

Assumed your playSMS is installed with these setups:

- Your playSMS web files is in `/home/user/web/playsms`
- Your playSMS database is `playsms`

Follow below steps in order:

1. Clone this repo to your playSMS server

   ```
   cd ~
   git clone https://github.com/playsms/plugin-uplink.git
   cd plugin-uplink
   ```

2. Copy gateway source to playSMS `plugin/gateway/`

   ```
   cp -rR src/uplink /home/user/web/playsms/plugin/gateway/
   ```

3. Restart `playsmsd`

   ```
   playsmsd restart
   playsmsd check
   ```
