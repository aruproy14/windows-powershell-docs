---
description: Use this topic to help manage Windows and Windows Server technologies with Windows PowerShell.
external help file: PS_BgpRouteAggregate_v1.0.cdxml-help.xml
Module Name: RemoteAccess
ms.date: 12/20/2016
online version: https://docs.microsoft.com/powershell/module/remoteaccess/set-bgprouteaggregate?view=windowsserver2022-ps&wt.mc_id=ps-gethelp
schema: 2.0.0
title: Set-BgpRouteAggregate
---

# Set-BgpRouteAggregate

## SYNOPSIS
Updates the properties of specified aggregate BGP route.

## SYNTAX

```
Set-BgpRouteAggregate [-RoutingDomain <String>] [-AttributePolicy <String[]>]
 [-PreserveASPath <PreserveASPath>] -Prefix <String> [-SummaryOnly <SummaryOnly>] [-PassThru] [-Force]
 [-CimSession <CimSession[]>] [-ThrottleLimit <Int32>] [-AsJob] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Set-BgpRouteAggregate** cmdlet updates the properties of specified aggregate Border Gateway Protocol (BGP) route.

## EXAMPLES

### Example 1: Update the custom route aggregation route properties
```
PS C:\>Set-BgpRouteAggregate -RoutingDomain "Contoso" -IPAddress "172.168.0.0" -PrefixLength 16 -SummaryOnly Enable -Force
```

This command updates the custom route aggregation route properties for routing domain named Contoso.

## PARAMETERS

### -AsJob
Runs the cmdlet as a background job. Use this parameter to run commands that take a long time to complete.

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

### -AttributePolicy
Specifies a string array of policy names that are to be applied to the aggregate route to configure its attributes.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -CimSession
Runs the cmdlet in a remote session or on a remote computer.
Enter a computer name or a session object, such as the output of a [New-CimSession](https://go.microsoft.com/fwlink/p/?LinkId=227967) or [Get-CimSession](https://go.microsoft.com/fwlink/p/?LinkId=227966) cmdlet.
The default is the current session on the local computer.

```yaml
Type: CimSession[]
Parameter Sets: (All)
Aliases: Session

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

### -Force
Indicates no confirmation prompt for updating aggregate route properties.

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

### -PassThru
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

### -Prefix
Specifies the classless IP address prefix for the aggregate IP address and its prefix length.

```yaml
Type: String
Parameter Sets: (All)
Aliases: AggregatePrefix

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PreserveASPath
Specifies a flag to keep the aggregated autonomous systems (AS) paths in the AS set of the aggregate IP address.

```yaml
Type: PreserveASPath
Parameter Sets: (All)
Aliases: 
Accepted values: Disabled, Enabled

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -RoutingDomain
Specifies a user-defined unique alphanumeric identifier for the routing.

```yaml
Type: String
Parameter Sets: (All)
Aliases: RoutingDomainName

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SummaryOnly
Specifies a flag that indicates that only the aggregate address is to be advertised to peers.

```yaml
Type: SummaryOnly
Parameter Sets: (All)
Aliases: 
Accepted values: Disabled, Enabled

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -ThrottleLimit
Specifies the maximum number of concurrent connections that can be established to run this command.
If you omit this parameter or enter a value of 0, the default value, 32, is used.

The throttle limit applies only to the current command, not to the session or to the computer.

```yaml
Type: Int32
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

### System.String

### System.String[]

### System.Nullable`1[[Microsoft.PowerShell.Cmdletization.GeneratedTypes.BgpRouteAggregate.PreserveASPath, Microsoft.PowerShell.Cmdletization.GeneratedTypes, Version=0.0.0.0, Culture=neutral, PublicKeyToken=null]]

### System.Nullable`1[[Microsoft.PowerShell.Cmdletization.GeneratedTypes.BgpRouteAggregate.SummaryOnly, Microsoft.PowerShell.Cmdletization.GeneratedTypes, Version=0.0.0.0, Culture=neutral, PublicKeyToken=null]]

## OUTPUTS

### Microsoft.Management.Infrastructure.CimInstance

### Microsoft.Management.Infrastructure.CimInstance#BgpRouteAggregateInfo

## NOTES

## RELATED LINKS

[Add-BgpRouteAggregate](./Add-BgpRouteAggregate.md)

[Get-BgpRouteAggregate](./Get-BgpRouteAggregate.md)

[Remove-BgpRouteAggregate](./Remove-BgpRouteAggregate.md)

[Remote Access Cmdlets](./remoteaccess.md)

