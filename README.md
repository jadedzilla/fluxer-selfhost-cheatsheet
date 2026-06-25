# The Fluxer Self Hosting Cheat Sheet

A helpful guide for common self hosting issues.

---

Table of Contents
- [The Fluxer Self Hosting Cheat Sheet](#the-fluxer-self-hosting-cheat-sheet)
    - [My custom assets aren't working!](#my-custom-assets-arent-working)
    - [I just finished the setup wizard, but I cant connect to any voice channels!](#i-just-finished-the-setup-wizard-but-i-cant-connect-to-any-voice-channels)

---

### My custom assets aren't working!
Add the file extension (.png) onto the end of the file url.

---

### I just finished the setup wizard, but I cant connect to any voice channels!

You will need to configure a Voice Region and server in the admin panel first.
1. Select **Voice Regions** from the sidebar.
2. Click **Create Region** and fill out the form to configure the region (tick **Set as default region** if you want that to be the default region) then click **Create Region**.
3. Refresh the page, and you should see your newly created region. Click **Manage Servers**.
4. Click **Add Server** and fill out the form. Use the API key and secret from the .env file. By default, the endpoint URL should be `wss://yourinstanceurl.com/livekit`.
5. Click **Add Server**. You're done! Try joining a voice channel, it should now successfully connect.

> [!important]
> It's important that the endpoint URL starts with `wss://` (instead of `https://` for example) and should end with `/livekit`. The only thing you should change is `yourinstanceurl.com`
