# How to Set Up a CS:GO Server on Linode

Setting up a Counter-Strike: Global Offensive (CS:GO) server on Linode can enhance your gaming experience by allowing you to customize game settings, play with friends, and manage your own private server. Follow this guide to get your CS:GO server up and running.

## Prerequisites
Before you start, ensure you have the following:
- A Linode account
- A Steam account (non-limited account)
- A Game Server Login Token
- CS:GO in your Steam library

## Steps

### On Steam

1. **Go to the Steam Game Server Management Page**
   - Visit [steamcommunity.com/dev/managegameservers](https://steamcommunity.com/dev/managegameservers).

2. **Login to Your Steam Account**
   - Enter your Steam credentials to log in.

3. **Generate a Game Server Login Token**
   - Type `730` for the App ID (CS:GO's App ID).
   - Add a memo as an identifier (this can be anything you want to name your server).
   - Click on "Create" to generate your login token.

4. **Copy Your Login Token**
   - Copy the token that is generated. You will need this token later.

### On Linode

1. **Access the Linode Marketplace**
   - Log in to your Linode account.
   - Go to the Marketplace tab and select "CS:GO".

2. **Enter Your Game Server Login Token**
   - Paste the login token you copied from Steam into the “Game Server Login Token” field.

3. **Set a Unique RCON Password**
   - Enter a secure RCON password. This password will be used to manage your server remotely.

4. **Configure Server Settings (Optional)**
   - Leave the default settings as they are unless you are familiar with the configurations and need to adjust them.

5. **Set a CS:GO Server Password (Optional)**
   - You can set a server password if you want to restrict access to your server.

6. **Select a Region**
   - Choose the region closest to you to minimize lag.

7. **Choose the Linode Size**
   - Depending on the number of players you plan on hosting, select an appropriate Linode size. The minimum recommended is 4GB.

8. **Set a Root Password**
   - Add a root password to secure your Linode and allow SSH access.

9. **Create Your Linode**
   - Click on “Create Linode” to launch your server.

### On CS:GO

1. **Enable the Developer Console**
   - Open CS:GO, go to Settings, and set "Enable Developer Console" to "Yes".

2. **Connect to Your Server**
   - Open the developer console in CS:GO by pressing the `~` key.
   - Type the following command to connect to your server:
     ```
     connect <IP address> password <CSGO server password>
     ```
   - Replace `<IP address>` with the IP address of your Linode server.
   - Replace `<CSGO server password>` with the password you set (if any).

3. **Start Playing!**
   - You are now connected to your CS:GO server. Enjoy your game!

By following these steps, you'll have your own CS:GO server up and running on Linode, allowing you to enjoy customized gameplay with your friends. Happy gaming!
