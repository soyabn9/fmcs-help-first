# Java FAQ

## Am I able to add a server icon to the server?

Yes, you are able to add a server icon to the server. Please upload a 64x64 png image named `server-icon.png` via FTP. Not sure which FTP and how to use it? Please follow [this](en/#how-to-get-and-use-the-recommended-ftp-client) guide.

## I am getting an Invalid Session / Invalid token / Failed to verify username error?

### Premium Account:

1. Close **ALL** minecraft related windows on your computer.
2. Then open minecraft again and try to join your server.

If this does not work try restarting your computer.

### Recent Minecraft Username Change:

1. Close **ALL** minecraft related windows on your computer.
2. Then open the launcher and log out and log back in.
3. Try to join the server.

### Cracked Account:

To resolve the error on a cracked account do the following:

1. Go to server.properties file in WebFTP
2. Find online-mode and set it to false
3. Restart your server and join.

If this does not work try to see if it is set to false in the server.properties file. If still does not work, contact support staff on [discord](https://discordapp.com/invite/u99dDtE) or create a ticket. A guide to creating a ticket is [here](en/#how-to-open-a-ticket).

## Adding a Custom IP to your Minecraft server:

> [!WARNING]
> This tutorial doesn't work on Bedrock/Windows 10/Pocket Edition servers! They don't support SRV records. 
>
> If you already own a domain on Freenom or any other domain registrar, you can skip some of the domain registration steps and when you get to changing Nameservers of the domain, if you are unsure how you do it on your domain registrar, Google can help you!
>
> IP won't change on the panel! You can use both old and the new IP you created with help of this tutorial to connect to your server.
>
> If you are doing this tutorial from a mobile phone or tablet, on the Cloudflare page after step number [**11)**](en/java-faq#step-11), make sure to click on the context menu of your browser (usually `...` three vertical dots) and check the `Request Desktop Site` option. If by any chance you don't have such option, use a computer or you can't complete all the steps successfully.

> [!DANGER]
> Beware, the server IP can change without warning. You will have to change the IP on the SRV record, if the server IP has changed.

### Step 1:

Get yourself a free domain from [https://freenom.com/](https://freenom.com/). *\"fmcshelptutorial.tk\" is just an example. Instead of it type in whatever you want your IP to be.*

![Freenom 1](../_images/custom-ip/Freenom-1.png 'Choose your domain')

### Step 2:

Change the duration of the domain from `3 Months` to `12 Months`.

![Freenom 2](../_images/custom-ip/Freenom-2.png 'Change the duration')

### Step 3:

Enter your email address and click `Verify My Email Address`.

![Freenom 3](../_images/custom-ip/Freenom-3.png 'Create an account')

### Step 4:

Open your email inbox in a new tab and open the email sent by Freenom. *If you don't see it, make sure to check "Spam" folder*. Click on the link to verify your email address.

![Freenom 4](../_images/custom-ip/Freenom-4.png 'Verify your account')

### Step 5:

On the next page enter any random info but your password and click the `Continue` button.

### Step 6:

Go to [https://cloudflare.com/](https://cloudflare.com/). Click `Sign up` button then register as usual.

### Step 7:

Click the `Add Site` button found on the home page.

![Cloudflare 1](../_images/custom-ip/Cloudflare-1.png 'Click the Add Site buttton')

### Step 8:

Replace `fmcshelptutorial.tk` with your domain (your new IP) you registered on [https://freenom.com/](https://freenom.com/).

![Cloudflare 2](../_images/custom-ip/Cloudflare-2.png 'Type your domain')

### Step 9:

Choose the `Free` plan and click `Confirm Plan` button.

![Cloudflare 3](../_images/custom-ip/Cloudflare-3.png 'Choose the Free plan')

### Step 10: 

This is where you will link your domain to your minecraft server.

![Cloudflare 4](../_images/custom-ip/Cloudflare-4.png)

### Step 11:

Change `A` to `SRV` Record

![Cloudflare 5](../_images/custom-ip/Cloudflare-5.png 'Choose SRV Record')

### Step 12:

**Type in following information:**

Service name: `_minecraft`

If you want to use `yourdomain.com` as your servers IP, type `@` in the **Name** field

or

For `play.yourdomain.com`, type `play` in the **Name** field

or

For `mc.yourdomain.com`, type `mc` in the **Name** field

or

You can type anything in **Name** field for example: If you type `something` you can use `something.yourdomain.com` to connect to your Minecraft server

If you want to use **yourdomain.com**, **play.yourdomain.com** as well as / or **mc.yourdomain.com**, repeat steps [**12)**](en/java-faq#step-12) - [**15)**](en/java-faq#step-15)

Click the `Save` button to continue.

![Cloudflare 6](../_images/custom-ip/Cloudflare-6.png 'Create SRV Record')

### Step 13:

Set the **priority** to `0` and the **weight** to `5` and continue to the next step without saving.

![Cloudflare 7](../_images/custom-ip/Cloudflare-7.png)

### Step 14:

Copy the Node DNS IP from your minecraft server and PORT and paste them in the correct area and click the `Save` button.

![Cloudflare 8](../_images/custom-ip/Cloudflare-8.png 'Copy and paste IP and PORT')

### Step 15:

Click the `Add Record` button and you will see it appear in the list below.

![Cloudflare 9](../_images/custom-ip/Cloudflare-9.png)
![Cloudflare 10](../_images/custom-ip/Cloudflare-10.png)

### Step 16:

After adding the SRV record and checking if everything is correct, click the `Continue` button.

![Cloudflare 11](../_images/custom-ip/Cloudflare-11.png)

### Step 17:

Go back to the Freenom site and click the `Manage Domain` button. *If you closed it, don't worry! Go to [https://my.freenom.com/clientarea.php?action=domains](https://my.freenom.com/clientarea.php?action=domains)*.

![Freenom 5](../_images/custom-ip/Freenom-5.png 'Managing your domain')

### Step 18:

Click on `Management Tools` and then `Nameservers`.

![Freenom 6](../_images/custom-ip/Freenom-6.png 'Adding custom Nameservers')

### Step 19:

Choose `use custom nameservers` on the Freenom site, copy over Nameserver 1 from Cloudflare to Freenom and do the same for Nameserver 2. Leave the other Nameservers blank, click the `Change Nameservers` button on the Freenom site, then click the `Done, check nameservers` button on the Cloudflare site.

![Cloudflare & Freenom 1](../_images/custom-ip/Cloudflare-Freenom-1.png 'Copying Nameservers to Freenom')

### Step 20:

Click the `Re-check now` button and wait at least an hour.

![Cloudflare 12](../_images/custom-ip/Cloudflare-12.png 'Re-check Now')

### Step 21:

Refresh your page and you will see the following. You might now be able to use your new IP.

![Cloudflare 13](../_images/custom-ip/Cloudflare-13.png 'Complete')

If you would like to check if your IP works. Go to [https://mcsrvstat.us/](https://mcsrvstat.us/) and type in your IP and click the  `Get server status` button. Click `Show debug info` for info on the hostname, IP, and port. 

![Minecraft Server Status 1](../_images/custom-ip/Minecraft-Server-Status-1.png 'Get Server Status')
![Minecraft Server Status 2](../_images/custom-ip/Minecraft-Server-Status-2.png 'Show Debug Info')
