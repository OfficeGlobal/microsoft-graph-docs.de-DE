# <a name="windowsdefenderscanactionresult-resource-type"></a>windowsDefenderScanActionResult-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Letzte Analyseergebnisse von Windows Defender

Erbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|actionName|Zeichenfolge|Aktionsname, geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|
|actionState|[actionState](../resources/intune_devices_actionstate.md)|Status der Aktion, geerbt aus [ DeviceActionResult.](../resources/intune_devices_deviceactionresult.md) Die möglichen Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|startDateTime|DateTimeOffset|Zeit, zu der die Aktion initiiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|
|lastUpdatedDateTime|DateTimeOffset|Zeit, zu der der Aktionszustand zuletzt aktualisiert wurde. Geerbt von [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|
|scanType|Zeichenfolge|Überprüfungstyp, entweder vollständige oder schnelle Überprüfung|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceActionResult",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```



