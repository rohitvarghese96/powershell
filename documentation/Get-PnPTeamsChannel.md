---
Module Name: PnP.PowerShell
title: Get-PnPTeamsChannel
schema: 2.0.0
applicable: SharePoint Online
external help file: PnP.PowerShell.dll-Help.xml
online version: https://pnp.github.io/powershell/cmdlets/Get-PnPTeamsChannel.html
---
 
# Get-PnPTeamsChannel

## SYNOPSIS

**Required Permissions**

  * Microsoft Graph API : One of Group.Read.All, Group.ReadWrite.All

Gets the channels for a specified Team.

## SYNTAX

```powershell
Get-PnPTeamsChannel -Team <TeamsTeamPipeBind> [-Identity <TeamsChannelPipeBind>] 
 [<CommonParameters>]
```

## DESCRIPTION

Allows to retrieve list of channels for a specified team.

## EXAMPLES

### EXAMPLE 1
```powershell
Get-PnPTeamsChannel -Team a6c1e0d7-f579-4993-81ab-4b666f8edea8
```

Retrieves all channels for the specified team

### EXAMPLE 2
```powershell
Get-PnPTeamsChannel -Team a6c1e0d7-f579-4993-81ab-4b666f8edea8 -Identity "Test Channel"
```

Retrieves the channel called 'Test Channel'

### EXAMPLE 3
```powershell
Get-PnPTeamsChannel -Team a6c1e0d7-f579-4993-81ab-4b666f8edea8 -Identity "19:796d063b63e34497aeaf092c8fb9b44e@thread.skype"
```

Retrieves the channel specified by its channel id

## PARAMETERS

### -Identity
The id or name of the channel to retrieve.

```yaml
Type: TeamsChannelPipeBind
Parameter Sets: (All)

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Team
Specify the group id, mailNickname or display name of the team to use.

```yaml
Type: TeamsTeamPipeBind
Parameter Sets: (All)

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

## RELATED LINKS

[Microsoft 365 Patterns and Practices](https://aka.ms/m365pnp)

