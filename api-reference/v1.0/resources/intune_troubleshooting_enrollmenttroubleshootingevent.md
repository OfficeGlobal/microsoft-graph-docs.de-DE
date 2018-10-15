# <a name="enrollmenttroubleshootingevent-resource-type"></a>enrollmentTroubleshootingEvent-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ereignis, das einen Fehler bei der Registrierung darstellt.

Erbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[EnrollmentTroubleshootingEvents auflisten](../api/intune_troubleshooting_enrollmenttroubleshootingevent_list.md)|[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)-Objekte.|
|[EnrollmentTroubleshootingEvent abrufen](../api/intune_troubleshooting_enrollmenttroubleshootingevent_get.md)|[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)|Lesen von Eigenschaften und Beziehungen des [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)-Objekts.|
|[EnrollmentTroubleshootingEvent erstellen](../api/intune_troubleshooting_enrollmenttroubleshootingevent_create.md)|[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)|Erstellen eines neuen [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)-Objekts.|
|[EnrollmentTroubleshootingEvent löschen](../api/intune_troubleshooting_enrollmenttroubleshootingevent_delete.md)|Keine|Löscht ein [enrollmentTroubleshootingEvent löschen](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)-Objekt.|
|[EnrollmentTroubleshootingEvent aktualisieren](../api/intune_troubleshooting_enrollmenttroubleshootingevent_update.md)|[enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)|Aktualisieren der Eigenschaften eines [enrollmentTroubleshootingEvent](../resources/intune_troubleshooting_enrollmenttroubleshootingevent.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|
|eventDateTime|DateTimeOffset|Uhrzeit, zu der das Ereignis aufgetreten ist. Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|
|correlationId|Zeichenfolge|ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde. Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|
|managedDeviceIdentifier|Zeichenfolge|Von Intune erstellter oder erfasster Gerätebezeichner|
|operatingSystem|Zeichenfolge|Betriebssystem|
|osVersion|Zeichenfolge|Betriebssystemversion|
|userId|Zeichenfolge|Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.|
|deviceId|Zeichenfolge|Azure AD-Gerätebezeichner|
|enrollmentType|[deviceEnrollmentType](../resources/intune_shared_deviceenrollmenttype.md)|Typ der Registrierung. Die möglichen Werte sind: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|failureCategory|[deviceEnrollmentFailureReason](../resources/intune_troubleshooting_deviceenrollmentfailurereason.md)|Allgemeine Fehlerkategorie. Die möglichen Werte sind: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.|
|failureReason|Zeichenfolge|Detaillierte Fehlerursache|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.deviceManagementTroubleshootingEvent",
  "@odata.type": "microsoft.graph.enrollmentTroubleshootingEvent"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "managedDeviceIdentifier": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "userId": "String",
  "deviceId": "String",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "String"
}
```



