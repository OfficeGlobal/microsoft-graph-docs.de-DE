# <a name="windowsinformationprotectiondesktopapp-resource-type"></a>windowsInformationProtectionDesktopApp-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Desktop-App für Windows-Informationsschutz

Erbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Anzeigename der App. Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|description|String|Die Beschreibung der App. Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|publisherName|String|Der Name des Herausgebers, geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|productName|String|Der Produktname. Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|denied|Boolean|Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert. Geerbt von [windowsInformationProtectionApp](../resources/intune_mam_windowsinformationprotectionapp.md)|
|binaryName|String|Der binäre Name|
|binaryVersionLow|String|Die niedrigere Binärversion.|
|binaryVersionHigh|String|Die größte Binärversion.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```



