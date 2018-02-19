# <a name="reportroot-resource-type"></a>reportRoot-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource, die eine Instanz der Verlaufsberichte darstellt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[reportRoot abrufen](../api/intune_deviceconfig_reportroot_get.md)|[reportRoot](../resources/intune_deviceconfig_reportroot.md)|Lesen von Eigenschaften und Beziehungen des [reportRoot](../resources/intune_deviceconfig_reportroot.md)-Objekts.|
|[reportRoot aktualisieren](../api/intune_deviceconfig_reportroot_update.md)|[reportRoot](../resources/intune_deviceconfig_reportroot.md)|Aktualisieren der Eigenschaften eines [reportRoot](../resources/intune_deviceconfig_reportroot.md)-Objekts.|
|[deviceConfigurationUserActivity-Funktion](../api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity.md)|[report](../resources/intune_deviceconfig_report.md)|Metadaten für den Gerätekonfigurations-Benutzeraktivitätsbericht|
|[deviceConfigurationDeviceActivity-Funktion](../api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity.md)|[report](../resources/intune_deviceconfig_report.md)|Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Der eindeutige Bezeichner für die Entität.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```



