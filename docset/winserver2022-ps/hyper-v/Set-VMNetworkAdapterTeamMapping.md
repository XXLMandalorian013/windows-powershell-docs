---
description: Use this topic to help manage Windows and Windows Server technologies with Windows PowerShell.
external help file: Microsoft.HyperV.PowerShell.Cmdlets.dll-Help.xml
Module Name: Hyper-V
ms.date: 12/20/2016
online version: https://learn.microsoft.com/powershell/module/hyper-v/set-vmnetworkadapterteammapping?view=windowsserver2022-ps&wt.mc_id=ps-gethelp
schema: 2.0.0
title: Set-VMNetworkAdapterTeamMapping
---

# Set-VMNetworkAdapterTeamMapping

## SYNOPSIS

## SYNTAX

### VMName (Default)
```
Set-VMNetworkAdapterTeamMapping [-CimSession <CimSession[]>] [-ComputerName <String[]>]
 [-Credential <PSCredential[]>] [-VMName] <String> [-VMNetworkAdapterName <String>]
 -PhysicalNetAdapterName <String> [-Passthru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ManagementOS
```
Set-VMNetworkAdapterTeamMapping [-ManagementOS] [-CimSession <CimSession[]>] [-ComputerName <String[]>]
 [-Credential <PSCredential[]>] [-VMNetworkAdapterName <String>] [-SwitchName <String>]
 -PhysicalNetAdapterName <String> [-Passthru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ResourceObject
```
Set-VMNetworkAdapterTeamMapping [-VMNetworkAdapter] <VMNetworkAdapterBase> -PhysicalNetAdapterName <String>
 [-Passthru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### VMObject
```
Set-VMNetworkAdapterTeamMapping [-VM] <VirtualMachine> [-VMNetworkAdapterName <String>]
 -PhysicalNetAdapterName <String> [-Passthru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Set-VMNetworkAdapterTeamMapping** cmdlet

## EXAMPLES

### Example 1
```powershell
Set-VMNetworkAdapterTeamMapping -VMName "Gateway01" -VMNetworkAdapterName "Internal NIC"
```

## PARAMETERS

### -CimSession
Runs the cmdlet in a remote session or on a remote computer.
Enter a computer name or a session object, such as the output of a [New-CimSession](https://go.microsoft.com/fwlink/p/?LinkId=227967) or [Get-CimSession](https://go.microsoft.com/fwlink/p/?LinkId=227966) cmdlet.
The default is the current session on the local computer.

```yaml
Type: CimSession[]
Parameter Sets: VMName, ManagementOS
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ComputerName
Specifies one or more Hyper-V hosts.
NetBIOS names, IP addresses, and fully qualified domain names are allowable.
The default is the local computer.
Use localhost or a dot (.) to specify the local computer explicitly.

```yaml
Type: String[]
Parameter Sets: VMName, ManagementOS
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
Parameter Sets: VMName, ManagementOS
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ManagementOS
Indicates that the cmdlet operates on the parent or host operating system.

```yaml
Type: SwitchParameter
Parameter Sets: ManagementOS
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Passthru
Returns an object representing the item with which you are working.
By default, this cmdlet does not generate any output.

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

### -PhysicalNetAdapterName
Specifies the name of the physical net adapter.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SwitchName
Specifies the name of a switch.

```yaml
Type: String
Parameter Sets: ManagementOS
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VM
Specifies a virtual machine.

```yaml
Type: VirtualMachine
Parameter Sets: VMObject
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -VMName
Specifies the name of a virtual machine.

```yaml
Type: String
Parameter Sets: VMName
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -VMNetworkAdapter
Specifies a virtual machine network adapter.

```yaml
Type: VMNetworkAdapterBase
Parameter Sets: ResourceObject
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -VMNetworkAdapterName
Specifies the name of a virtual network adapter.

```yaml
Type: String
Parameter Sets: VMName, ManagementOS, VMObject
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

### Microsoft.HyperV.PowerShell.VMNetworkAdapterTeamMappingSetting

## NOTES

## RELATED LINKS

[Get-VMNetworkAdapterTeamMapping](./Get-VMNetworkAdapterTeamMapping.md)

[Remove-VMNetworkAdapterTeamMapping](./Remove-VMNetworkAdapterTeamMapping.md)

