Welcome to Git Drive
=================================
Git Drive is a system especially designed for iOS，enabling Git version control software to be operated on mobile devices, by which your iOS device becomes a perfectly functioning Git version control server that fits in the palm of your hand. All you only need to do is install the application from the Apple App Store; there is no tedious, multi-step installation process or any further effort required – a Git version control server will be set up within minutes. The Git Smart transfer protocol is fully implemented on this server, including transmission stability and speed. Authorization of other users for repository access is under your complete control, and shallow updates and cloning operations for the repository are also supported.

Because of Git’s distributed architecture, damage at a singular location will not lead to an entire system breakdown; in this way, Git Drive is extremely suitable for use as a node within a Git storage network – and this node can be carried with you wherever you go. 

Besides acting as a perfectly functioning Git version control server, the Git Drive software also acts as a powerful Git client, offering enough functionality for you to effectively manage changes to the repository and check up on any documents directly from the application.

Git Drive offers a different way to manage your code other than conventional code-management models. For example, when using Git Drive, your code is stored on your personal device – and if you are also using iCloud, any repository can be available on any device, step-by-step and in real time. Only through this model are you able to fully utilize the available space on your iPhone or iPad as storage for all of your important data. It facilitates convenient data exchange among a working team, while at the same time saving you the cost and time of setting up a personal Git version control server.

## Quick Start
#### What is Git?
If you are not already familiar with Git, here is an online tutorial to help you get started with Git faster [A great online Git tutorial](https://git-scm.com/book/en/v2)
#### How to Transfer Existing Local Repositories to Git Drive
- Ensure that your mobile device and PC are connected to the same Wi-Fi network.
- Open Git Drive, and confirm that the Git server is in the "Enabled" state. If enabled, the Server switch will be blue ***(Side Menu --> Server Switch)***.
- Open the Git Drive Finder, allowing the Finder to map the Git Drive domain for you.
- In ***Create New Repository*** screen ***(Left Menu --> All Repositories --> Create New Repositories)***, input ***myrepo*** and click to complete.
- After entering the local Git repository, input the following command to finish adding the remote Git repository:

```
git remote add myrepo http://gitdrive.com/myrepo
```
- Finally, input the following command to push the local repository to Git Drive:

```
git push myrepo refs/heads/*:refs/heads/*
```
#### How to Clone a Repository from Git Drive
- Ensure that your mobile device and PC are connected to the same Wi-Fi network.
- Open Git Drive, and confirm that the Git server is in the "Enabled" state. If enabled, the Server switch will be blue ***(Side Menu --> Server Switch)***.
- Open the Git Drive Finder, allowing the Finder to map the Git Drive domain for you.
- From here, enter the following command to establish a new repository:

```
git clone http://gitdrive.com/your_repo_name
```

- Or, to establish a shallow repository, enter the following command:

```
git clone —-depth=1 http://gitdrive.com/your_repo_name
```

#### Git Drive Finder

Because you may be switching between different network connections, we suggest that you access your server using a domain name. To avoid having to modify the Host file each time you switch networks, we have developed Git Drive Finder(located in the /Tutorial/finder directory). This tool uses Java, so there are no system restrictions for its use.

Git Drive Finder will automatically locate Git Drive within a network, and add a domain name and IP mapping to the Host file. From a security standpoint, we require that the device passcode be provided ***(Side Menu --> Right Side of IP Address)***. After entering the device passcode, click ***START*** to begin a search; only devices with that passcode will be found. Please ensure that Git Drive is open before beginning a search.

Because this automatic configuration tool needs to modify the system’s Host file, Administrator Authorization is required for use in Windows systems. Mac systems, along with other Unix or Linux systems, need to use sudo to run the tool; otherwise it will be unable to modify the Host file.

Navigate to ***Side Menu --> Settings --> Server*** to configure the server domain name. After configuration is complete, you will only need to run Finder when switching network connections, and the IP address corresponding to your domain name will be automatically updated on your computer.

Table of Contents
=================================
- [Managing Repositories](./docs/chapter_1_en.md)
- [Viewing Repository Content](./docs/chapter_2_en.md)
- [Commit History](./docs/chapter_3_en.md)
- [Git Server Management](./docs/chapter_4_en.md)

