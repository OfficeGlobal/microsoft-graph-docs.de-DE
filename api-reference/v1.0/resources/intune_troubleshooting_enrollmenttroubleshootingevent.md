# <a name="enrollmenttroubleshootingevent-resource-type"></a>enrollmentTroubleshootingEvent-Ressourcentyp

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
|id|String|UUID für das Objekt. Geerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|
|eventDateTime|DateTimeOffset|Uhrzeit, zu der das Ereignis aufgetreten ist. Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|
|correlationId|String|ID, die für die Verfolgung des Fehlers in dem Dienst verwendet wurde. Gerbt von [deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)|
|managedDeviceIdentifier|String|Von Intune erstellter oder erfasster Gerätebezeichner|
|operatingSystem|String|Betriebssystem|
|osVersion|String|Betriebssystemversion|
|userId|String|Bezeichner für den Benutzer, der versucht hat, das Gerät zu registrieren.|
|deviceId|String|Azure AD-Gerätebezeichner|
|enrollmentType|String|Typ der Registrierung. Mögliche Werte: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|failureCategory|String|Allgemeine Fehlerkategorie. Mögliche Werte: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`.|
|failureReason|String|Detaillierte Fehlerursache|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentTroubleshootingEvent"
}
-->
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



