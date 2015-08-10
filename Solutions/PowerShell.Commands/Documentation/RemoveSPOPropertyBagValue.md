#Remove-SPOPropertyBagValue
*Topic automatically generated on: 2015-07-08*

Removes a value from the property bag
##Syntax
```powershell
Remove-SPOPropertyBagValue [-Folder <String>] [-Force [<SwitchParameter>]] [-Web <WebPipeBind>] -Key <String>
```


##Parameters
Parameter|Type|Required|Description
---------|----|--------|-----------
|Folder|String|False|Site relative url of the folder. See examples for use.|
|Force|SwitchParameter|False||
|Key|String|True||
|Web|WebPipeBind|False|The web to apply the command to. Omit this parameter to use the current web.|
##Examples

###Example 1
    PS:> Remove-SPOPropertyBagValue -Key MyKey
This will remove the value with key MyKey from the current web property bag

###Example 2
    PS:> Remove-SPOPropertyBagValue -Key MyKey -Folder /MyFolder
This will remove the value with key MyKey from the folder MyFolder which is located in the root folder of the current web

###Example 3
    PS:> Remove-SPOPropertyBagValue -Key MyKey -Folder /
This will remove the value with key MyKey from the root folder of the current web
<!-- Ref: 78282DCDA2059ED043399AA32D80EF36 -->