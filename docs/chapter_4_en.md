Git Server Management
=================================

#### Accessing a Remote Repository 
GitDrive acts as a perfectly functioning Git version control server. Once your device is connected to a Wi-Fi network and GitDrive is opened, the server will automatically be activated, allowing you to push or pull your repositories using either Http or Git protocols. Note that if a repository is already enabled for remote user authorization, Git protocol cannot be used, since Git protocol does not support user authorization.

Navigate to ***Side Menu --> Settings --> Server*** to configure the Http and Git protocols. Changes will be effective immediately – there is no need for any additional work on your part. 

The blue button located at the top of the Side Menu is the Server switch. Clicking this switch will activate or deactivate the server. Underneath the switch, your device’s IP address is shown; supposing that your IP address is ***192.168.1.100***, and your repository is named ***myrepo***, your repository can be cloned with one of the following commands:
```
git clone http://192.168.1.100/myrepo OR
git clone git://192.168.1.100/myrepo
```

#### Background Operation Mode

Under the default setting, the GitDrive will continue to operate for a set period of time (a few minutes) after exiting to the home screen or switching to another application. The Git server will remain connected during this period of time.

If you disable Background Operation Mode from the Server Settings, the Git server will stop working when you exit to the device home screen or switch to another application – you will have no way to connect your device unless you re-open GitDrive.


