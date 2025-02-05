---
description: Use this topic to help manage Windows and Windows Server technologies with Windows PowerShell.
external help file: Microsoft.HyperV.PowerShell.Cmdlets.dll-Help.xml
Module Name: Hyper-V
ms.date: 12/20/2016
online version: https://learn.microsoft.com/powershell/module/hyper-v/get-vmremotefxphysicalvideoadapter?view=windowsserver2022-ps&wt.mc_id=ps-gethelp
schema: 2.0.0
title: Get-VMRemoteFXPhysicalVideoAdapter
---

# Get-VMRemoteFXPhysicalVideoAdapter

## SYNOPSIS
Gets the RemoteFX physical graphics adapters on one or more Hyper-V hosts.

## SYNTAX

### ComputerName (Default)
```
Get-VMRemoteFXPhysicalVideoAdapter [-ComputerName <String[]>] [-Credential <PSCredential[]>]
 [[-Name] <String[]>] [<CommonParameters>]
```

### CimSession
```
Get-VMRemoteFXPhysicalVideoAdapter [-CimSession <CimSession[]>] [[-Name] <String[]>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-VMRemoteFXPhysicalVideoAdapter** cmdlet gets the RemoteFX physical graphics adapters on one or more Hyper-V hosts.

## EXAMPLES

### Example 1
```powershell
Get-VMRemoteFXPhysicalVideoAdapter
```

Gets all RemoteFX physical video adapters on the Hyper-V host.

### Example 2
```powershell
Get-VMRemoteFXPhysicalVideoAdapter -Name *Nvidia*
```

Gets all RemoteFX physical video adapters on the Hyper-V host which include the sequence Nvidia in their name.

## PARAMETERS

### -CimSession
Runs the cmdlet in a remote session or on a remote computer.
Enter a computer name or a session object, such as the output of a [New-CimSession](https://go.microsoft.com/fwlink/p/?LinkId=227967) or [Get-CimSession](https://go.microsoft.com/fwlink/p/?LinkId=227966) cmdlet.
The default is the current session on the local computer.

```yaml
Type: CimSession[]
Parameter Sets: CimSession
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ComputerName
Specifies one or more Hyper-V hosts that run this cmdlet.
NetBIOS names, IP addresses, and fully qualified domain names are allowable.
The default is the local computer.
Use localhost or a dot (.) to specify the local computer explicitly.

```yaml
Type: String[]
Parameter Sets: ComputerName
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Credential
Specifies one or more user accounts that have permission to perform this action.
The default is the current user.

```yaml
Type: PSCredential[]
Parameter Sets: ComputerName
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the names of one or more RemoteFX physical graphics adapters to be retrieved.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.HyperV.PowerShell.VMRemoteFXPhysicalVideoAdapter

## NOTES

## RELATED LINKS

