Git Server Management
=================================

#### Accessing a Remote Repository 
Git Drive acts as a perfectly functioning Git version control server. Once your device is connected to a Wi-Fi network and Git Drive is opened, the server will automatically be activated, allowing you to push or pull your repositories using either Http or Git protocols. Note that if a repository is already enabled for remote user authorization, Git protocol cannot be used, since Git protocol does not support user authorization.

Navigate to ***Side Menu --> Settings --> Server*** to configure the Http and Git protocols. Changes will be effective immediately – there is no need for any additional work on your part. 

The blue button located at the top of the Side Menu is the Server switch. Clicking this switch will activate or deactivate the server. Underneath the switch, your device’s IP address is shown; supposing that your IP address is ***192.168.1.100***, and your repository is named ***myrepo***, your repository can be cloned with one of the following commands:
```
git clone http://192.168.1.100/myrepo OR
git clone git://192.168.1.100/myrepo
```



