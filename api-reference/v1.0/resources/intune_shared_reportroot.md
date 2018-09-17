# <a name="reportroot-resource-type"></a>reportRoot-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Die Ressource, die eine Instanz der Verlaufsberichte darstellt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[reportRoot abrufen](../api/intune_shared_reportroot_get.md)|[reportRoot](../resources/intune_shared_reportroot.md)|Lesen von Eigenschaften und Beziehungen des [reportRoot](../resources/intune_shared_reportroot.md)-Objekts.|
|[reportRoot aktualisieren](../api/intune_shared_reportroot_update.md)|[reportRoot](../resources/intune_shared_reportroot.md)|Aktualisieren der Eigenschaften eines [reportRoot](../resources/intune_shared_reportroot.md)-Objekts.|
|**deviceConfiguration**|
|[deviceConfigurationDeviceActivity-Funktion](../api/intune_shared_reportroot_deviceconfigurationdeviceactivity.md)|[Bericht](../resources/intune_shared_report.md)|Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht|
|[deviceConfigurationUserActivity-Funktion](../api/intune_shared_reportroot_deviceconfigurationuseractivity.md)|[Bericht](../resources/intune_shared_report.md)|Metadaten für den Gerätekonfigurations-Benutzeraktivitätsbericht|
|**Problembehandlung**|
|[ManagedDeviceEnrollmentFailureDetails-Funktion](../api/intune_shared_reportroot_manageddeviceenrollmentfailuredetails.md)|[Bericht](../resources/intune_shared_report.md)|Noch nicht dokumentiert.|
|[ManagedDeviceEnrollmentTopFailures-Funktion](../api/intune_shared_reportroot_manageddeviceenrollmenttopfailures.md)|[Bericht](../resources/intune_shared_report.md)|Noch nicht dokumentiert.|


## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Der eindeutige Bezeichner für die Entität.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a>Beispiel

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```