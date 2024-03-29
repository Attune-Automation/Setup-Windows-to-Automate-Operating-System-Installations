



[![Docs](https://img.shields.io/badge/docs-latest-brightgreen.svg)](http://doc.servertribe.com)
[![Discord](https://img.shields.io/discord/844971127703994369)](http://discord.servertribe.com)
[![Docs](https://img.shields.io/badge/videos-watch-brightgreen.svg)](https://www.youtube.com/@servertribe)
[![Generic badge](https://img.shields.io/badge/download-latest-brightgreen.svg)](https://www.servertribe.com/community-edition/)

# Setup Windows to Automate Operating System Installations

Attune provides a solution to streamline the OS installation process.

This Attune Project sets up a Windows machine as a worker for automating 
operating system installations.

## What is a worker?

The majority of the workload creating the ISO file(s) 
is performed on either the Attune host machine or a separate machine. This 
machine is referred to as the worker.

The workload covers tasks such as unpacking ISO, repackaging with the drivers 
and configurations, deploying files to the controller, and triggering APIs on 
the controller.

## Documentation

[Automate Operating System Installation](https://docs.attuneautomation.com/en/latest/topics/automated_os_installation.html)




# Attune

[Attune](https://www.servertribe.com/)
automates and orchestrates processes to streamline deployments, scaling,
migrations, and management of your systems. The Attune platform is building a
community of sharable automated and orchestrated processes.

You can leverage the publicly available orchestrated blueprints to increase
your productivity, and accelerate the delivery of your projects. You can
open-source your own work and improve existing community orchestrated projects.

## Get Started with Attune, Download NOW!

The **Attune Community Edition** can be
[downloaded](https://www.servertribe.com/comunity-edition/)
for free from our
[ServerTribe website](https://www.servertribe.com/comunity-edition/).
You can learn more about Attune through
[ServerTribe's YouTube Channel](https://www.youtube.com/@servertribe).







# Clone this Project

To clone this project into your own instance of Attune, follow the
[Clone a GIT Project How To Instructions](https://servertribe-attune.readthedocs.io/en/latest/howto/design_workspace/clone_project.html).




## Blueprints

This Project contains the following Blueprints.



### Setup Windows Worker for WinPE ISOs Installations

The scripts within each step automate the Windows worker setup for automating 
Windows installation using WinPE ISOs.

#### Install Windows Assessment and Deployment Kit (ADK)
Download and install the appropriate ADK and WinPE Add-On version based on the 
Windows distribution.

#### Install Worker Prerequisites on Windows
Download and install 7z.

#### Setup and Create SmbShare Folder on Windows
Enable the File and Printer Sharing service, 
configure the firewall for Network Discovery, 
create an SMB share folder, and 
setup appropriate NTFS permissions.

### Install Windows Assessment and Deployment Kit

The Windows Assessment and Deployment Kit (Windows ADK) and 
Windows PE add-on has the tools you need to customise 
Windows images for large-scale deployment, and to test 
the quality and performance of your system, its added 
components, and the applications running on it.

[Microsoft Documentation](https://learn.microsoft.com/en-us/windows-hardware/get-started/adk-install)

### Create a SMB Share folder

Create a shared space for storing and accessing files.

SMB (Server Message Block) is widely supported and provides a flexible way 
to connect different devices and operating systems for file sharing.

This process includes:
* Enable the File and Printer Sharing service, 
* configure the firewall for Network Discovery, 
* create an SMB share folder, 
* setup appropriate NTFS permissions, and 
* Turn off password protected sharing (optional).




## Parameters


| Name | Type | Script Reference | Comment |
| ---- | ---- | ---------------- | ------- |
| Automation Worker Windows Base Directory | Text | `automationworkerwindowsbasedirectory` | Base directory for deploying temporary files to build the ISO on a Windows Worker.<br><br>eg. "C:/attune_auto_installer" |
| Automation Worker Windows Node | Windows Node | `automationworkerwindowsnode` | The Windows automation worker node used to perform tasks to create the ISO. |
| Automation Worker Windows User: Administrator | Windows Credential | `automationworkerwindowsuseradministrator` | Administrator user on the Windows Automation Worker node. |




## Files

| Name | Type | Comment |
| ---- | ---- | ------- |






# Contribute to this Project

**The collective power of a community of talented individuals working in
concert delivers not only more ideas, but quicker development and
troubleshooting when issues arise.**

If you’d like to contribute and help improve these projects, please fork our
repository, commit your changes in Attune, push you changes, and create a
pull request.

<img src="https://www.servertribe.com/wp-content/uploads/2023/02/Attune-pull-request-01.png" alt="pull request"/>

---

Please feel free to raise any issues or questions you have.

<img src="https://www.servertribe.com/wp-content/uploads/2023/02/Attune-get-help-02.png" alt="create an issue"/>


---

**Thank you**
