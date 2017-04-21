Managing Repositories
=================================
Since mobile devices are powered solely through their batteries, unlike other computing devices which constantly receive power through a main power source, low battery charge while on the go can become a problem. Low power can lead to system shut-downs, and interruptions can also be caused by incoming phone calls, and more. Because our user’s data security is of the utmost importance to us, particular consideration was given to this potential issue during design.

Any repository-related operations are atomic, which is to say if an operation is interrupted or fails, the repository will roll back to its prior state before that operation, and there will be no effect on the repository’s data as a whole.

Repository management is accomplished while in the ***All Repositories*** view, reached via ***Side Menu --> All Repositories***.

Establishing a New Repository
---------
#### Setting Up an Empty Repository
Click on the ***Create New Repository*** button to open the New Repository view, and after entering the desired repository name click ***Done***. Any repository created through this method will be automatically synced to iCloud by default, and any future updates to the repository will be automatically synced to iCloud as well.

#### Cloning a Remote Repository
Use this function to clone a repository located on a remote server. Click on the ***Clone From URL*** button to open the Clone Repository view, and after inputting the complete URL of the repository you wish to clone, click ***Done***. Any repository created through this method will be automatically synced to iCloud by default, and any future updates to the repository will be automatically synced to iCloud as well.

If authorization is required to clone the remote repository, you must provide the correct username and password before the repository will begin cloning.

Via the Task view ***(Side Menu --> Tasks)***, you can check on the download progress of any cloned repositories, or cancel any cloned repositories mid-download. 

#### Downloading from GitHub
Besides the methods mentioned above, Git Drive also supports a search function for repositories on GitHub, allowing you to locate and download your desired GitHub repository directly from the application. By default, any repositories downloaded from GitHub will not be synced to iCloud. If you want to upload these repositories to iCloud, you must manually change this setting after downloading. 

As the default setting, all currently downloading repositories will pause after exiting to the home screen or entering another application. Enable the setting for Background Operation Mode, found within the Server Settings menu ***(Side Menu -->  Settings --> Server)***, to continue a download until its completion, regardless of whether or not you are still in the app.

It is suggested that this function remain disabled for most downloads, due to the limitations of mobile device processing capabilities; too many downloads may lead to excessive use of resources by the application, causing Git Drive to be shut down by the system.

Deleting a Repository
---------
Within the ***All Repositories*** view, click on the ***Edit*** button in the upper right corner of the screen. The repository list will switch to editing mode. Find the repository you wish to delete, and click on the gray Trash button to its left. Before deleting, ensure that the selected repository will no longer be needed – this operation will also delete any duplicates already uploaded to the Cloud. Deletions are irreversible, so always use extreme caution when deleting! 

If the deleted repository is also synchronized to other devices, it will not be automatically deleted from those devices; however, the Cloud Synchronization option for this repository will be disabled to prevent it from being re-uploaded to the Cloud.

Setting Up a Repository
---------
Within the ***All Repositories*** view, click on the ***Edit*** button in the upper right corner of the screen. The repository list will switch to editing mode. Find the repository you wish to modify, and click on the blue Settings button to its right. You will be taken to the repository setting screen, from which you can modify any of the following items as they relate to the selected repository:
- Name the repository
- Enable/disable Cloud synchronization
- Allow shallow updates to the repository
- Allow remote access to the repository
- Authorize remote users

#### Enabling Cloud Synchronization
After enabling this setting, any content updates to a repository will be automatically synchronized with iCloud, up until the setting is disabled. Once disabled, any duplicates of the repository already synchronized with iCloud will also be deleted, to free up additional space on your iCloud account.

#### Allowing Shallow Updates to a Repository
If your local repository was not cloned in shallow mode, then it will not receive shallow updates, unless the ***–depth*** parameter was added at the time of cloning.  This could cause a shallow repository, if you don’t introduce any shallow updates until the push to Git Drive; shallow updates are allowed by default.

#### Allowing Remote Access to a Repository
Disabling this option will cause a repository to become inaccessible to remote users.

#### Authorizing Remote Users
If this option is enabled, any remote users will need to provide a username and password to complete authorization for remote access to a repository.

You will need to assign authorized users for a repository while on the ***User Management*** screen; if a repository does not have any authorized users, there will be no way for remote users to access it. After enabling authorized user access, click ***User Management*** Options to select which users have permission to access the repository. 


