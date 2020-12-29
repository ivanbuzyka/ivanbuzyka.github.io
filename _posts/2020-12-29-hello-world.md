---
title: Hello World
---

Below is some test syntax

```
param(	[string] $ResourceGroupName = "rgname",	
	[string] $WebAppName = "webappname",
	[string] $StorageAccountSasUrl = "",
	[string] $BackupName = "backupname"
    )
	
	Write-Host "Restoring $WebAppName from $StorageAccountSasUrl..."
	Restore-AzWebAppBackup -ResourceGroupName $ResourceGroupName -Name $WebAppName -StorageAccountUrl $StorageAccountSasUrl -BlobName $BackupName -Overwrite
	
	Write-Host "Backup restoring scheduled..."
```
