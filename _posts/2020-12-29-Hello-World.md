---
layout: post
date: 2020-12-29 11:45:00 +0100
categories: Sitecore
---

## Hey, this is a new thing!

Below is some test syntax

```PowerShell
param(	[string] $ResourceGroupName = "rgname",	
	[string] $WebAppName = "webappname",
	[string] $StorageAccountSasUrl = "",
	[string] $BackupName = "backupname"
    )
	
	Write-Host "Restoring $WebAppName from $StorageAccountSasUrl..."
	Restore-AzWebAppBackup -ResourceGroupName $ResourceGroupName -Name $WebAppName -StorageAccountUrl $StorageAccountSasUrl -BlobName $BackupName -Overwrite
	
	Write-Host "Backup restoring scheduled..."
```
