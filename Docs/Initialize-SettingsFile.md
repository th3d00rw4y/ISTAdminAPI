Initialize-SettingsFile
===================

## SYNOPSIS
Build a settings file and store it on the computer.

## SYNTAX
```powershell
Initialize-SettingsFile [[-Server] <String>] [-CustomerID] <String> [<CommonParameters>]
```

## DESCRIPTION
This CMDlet will build a CSV file with information on how to connect to your organizations instance of ISTAdmin.
You will also be prompted to select your credential file. If you haven't generated a credential file, please refer to the module documentation.
Lastly you will be prompted to select a folder where the settings file will be stored.

## PARAMETERS
### -Server &lt;String&gt;
Your organizations API instance of ISTAdmin. e.g: https://api.ist.com/ss12000v2-api/source/<Your customer Id>/v2.0
This parameter is by default hidden and pre populated with the server adress to the EduCloud API
```
Required?                    false
Position?                    1
Default value                https://api.ist.com/ss12000v2-api/source/<REPLACE>/v2.0
Accept pipeline input?       false
Accept wildcard characters?  false
```
 
### -CustomerID &lt;String&gt;
Your customer id eg. "SE00100"
```
Required?                    true
Position?                    2
Default value
Accept pipeline input?       false
Accept wildcard characters?  false
```

## INPUTS


## OUTPUTS


## NOTES
Author: Simon Mellergård | IT-avdelningen, Värnamo kommun

## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>Initialize-SettingsFile -CustomerID "SE00100"

# This will give you two different prompts. First one you will have to select the folder where the CSV file are to be stored. Second prompt will ask for the encrypted credential file holding you credentials.
```


