---
layout: post
title: "How to Update Debian and Windows on CLI"
date: 2022-12-16 09:00:00 -0500
categories: [windows,linux]
tags: [bash,powershell]
---

# How to Update Debin and Windows on CLI 

## Debian

If you want to update debian using the CLI you can use the following command

```bash
sudo apt update && sudo apt upgrade -y
```

that willto do the followin:

* check for updates
* download the updates 
* auto install the upgrades

you can separate this by runnding the follwing

```bash
sudo apt update
```

```bash
sudo apt upgrade
```

## Windows

### To update installed applications

search for updates

```powershell
winget upgrade
```
update all apps
```powershell
winget upgrade -h --all
```
update an app using the app ID
```powershell
winget upgrade -e --ID TeamViewer.TeamViewer
```
### To install Windows Updates

install the Powershell Module
```powershell
Install-Module PSWindowsUpdate
```
seach for updates
```powershell
Get-WindowsUpdate
```
install the updates
```powershell
Install-WindowsUpdate
```

I hope this is helpful. 
