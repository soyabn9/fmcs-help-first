# Java Plugin FAQ

> [!DANGER]
> THIS PAGE IS NOT YET COMPLETE!

> [!WARNING]
> Before you go and read this FAQ, the following information may change without warning. Now that you have been warned carry on.

## My server got suspended for a plugin I bought?

The server does not know if a user buys a plugin, so to be able to use the plugin that you have bought, you have to be whitelisted for that plugin. There is instruction below on how to verify the plugin is bought.

### How to join the plugin whitelist:

Send a message to the plugin developer to send a message to [Facha](https://www.spigotmc.org/members/esquilo_azul.19239/) \(Owner\). The message sent from the plugin developer must include:

* Your freemcserver.net username EXAMPLE: Minecraftpro1234
* Where you are going to use it EXAMPLE: freemcserver.net
* The plugin name/link EXAMPLE: featherboard
* The plugin hash for the version that is used \(The plugin developer should know this\)

As soon as [Facha](https://www.spigotmc.org/members/esquilo_azul.19239/) \(Owner\) gets the message via spigot which his username can be found by clicking his name. The person then gets the email saying he is whitelisted and is then allowed use the plugin. Further servers on the account, do not need to repeat the process. It is once per user per plugin.

## How to setup the Dynamic Map Plugin?

1. Download the DynMap Plugin \([LINK](https://www.spigotmc.org/resources/dynmap.274/)\)
2. Upload the plugin to the server like any other plugin. Tutorial here: [LINK](https://youtu.be/QRldgu51qJg)
3. Start the server to generate all the files
4. Replace [this](https://cdn.discordapp.com/attachments/586568892810526720/647837234216828941/configuration.txt) configuration file with the existing one
5. Find and replace `webserver-port` number to a range between `50000 - 51000`
6. Start the server and locate the following in the console:

```text
15.11 16:59:53 [Server] INFO [16:59:53 INFO]: [dynmap] Web server started on address SERVER-IP:WEBSERVER-PORT
```

7. Go to `SERVER-IP:WEBSERVER-PORT` in a new tab, replacing `SERVER-IP` with your own server IP and `WEBSERVER-PORT` with the number you chose in the config file

> [!NOTE]
> SERVER-IP can either be the IP shown in console \(Example: `136.243.71.281`\) or the Node DNS of your server \(Example: `helios.freemcserver.net`\).
> 
> DynMap is best used with a MySQL database as it can load faster. A guide will come soon.
