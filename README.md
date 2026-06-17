## The Fluxer Self Hosting Cheat Sheet
###### A helpful guide for common self hosting issues.

<details>
  <summary>My custom assets aren't working</summary>

  Add the file extension (.png) onto the end of the file url.
</details>
<details>
  <summary>I just finished the setup wizard, but I cant connect to any voice channels!</summary>
  
##### You will need to configure a Voice Region and server in the admin panel first.
1. Select "Voice Regions" from the sidebar.
2. Click "Create Region" and fill out the form to configure the region (tick "Set as default region" if you want that to be the default region) then click "Create Region".
3. Refresh the page, and you should see your newly created region. Click "Manage Servers".
4. Click "Add Server" and fill out the form. Use the API key and secret from the .env file. By default, the endpoint URL should be wss://yourinstanceurl.com/livekit.
5. Click "Add Server". You're done! Try joining a voice channel, it should now successfully connect.
</details>
