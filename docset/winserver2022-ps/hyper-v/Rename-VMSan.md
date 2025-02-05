---
description: Use this topic to help manage Windows and Windows Server technologies with Windows PowerShell.
external help file: Microsoft.HyperV.PowerShell.Cmdlets.dll-Help.xml
Module Name: Hyper-V
ms.date: 12/20/2016
online version: https://learn.microsoft.com/powershell/module/hyper-v/rename-vmsan?view=windowsserver2022-ps&wt.mc_id=ps-gethelp
schema: 2.0.0
title: Rename-VMSan
---

# Rename-VMSan

## SYNOPSIS
Renames a virtual storage area network (SAN).

## SYNTAX

```
Rename-VMSan [-CimSession <CimSession[]>] [-Name] <String> [-NewName] <String> [-Passthru]
 [-ComputerName <String[]>] [-Credential <PSCredential[]>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Rename-VMSan** cmdlet renames a virtual storage area network (SAN).

## EXAMPLES

### Example 1
```powershell
Rename-VMSan -Name Production -NewName Test
```

Renames a virtual storage area network from Production to Test.

## PARAMETERS

### -CimSession
Runs the cmdlet in a remote session or on a remote computer.
Enter a computer name or a session object, such as the output of a [New-CimSession](https://go.microsoft.com/fwlink/p/?LinkId=227967) or [Get-CimSession](https://go.microsoft.com/fwlink/p/?LinkId=227966) cmdlet.
The default is the current session on the local computer.

```yaml
Type: CimSession[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ComputerName
Specifies the name of the Hyper-V host on which the virtual storage area network (SAN) is to be renamed.
NetBIOS names, IP addresses, and fully qualified domain names are allowable.
The default is the local computer.
Use localhost or a dot (.) to specify the local computer explicitly.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential
Specifies one or more user accounts that have permission to perform this action.
The default is the current user.

```yaml
Type: PSCredential[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the current name of the virtual storage area network (SAN) to be renamed.

```yaml
Type: String
Parameter Sets: (All)
Aliases: SanName

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -NewName
Specifies the new name of the virtual storage area network (SAN) to be renamed.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Passthru
Specifies that an object is to be passed through to the pipeline representing the renamed virtual storage area network (SAN).

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](https://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### None
Default

### Microsoft.HyperV.PowerShell.VMSan
If **-PassThru** is specified.

## NOTES

## RELATED LINKS

