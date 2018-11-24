# <a name="user-resource-type"></a>user-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt ein user-Objekt von Azure Active Directory dar.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste Benutzer](../api/intune_shared_user_list.md) -Objekte.|[user](../resources/intune_shared_user.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune_shared_user.md)-Objekte.|
|[Abrufen von Benutzer](../api/intune_shared_user_get.md) -Objekt.|[Benutzersammlung](../resources/intune_shared_user.md)|Lesen von Eigenschaften und Beziehungen des [user](../resources/intune_shared_user.md)-Objekts.|
|[Create User](../api/intune_shared_user_create.md) -Objekt.|[Benutzersammlung](../resources/intune_shared_user.md)|Dient zum Erstellen eines neuen [user](../resources/intune_shared_user.md)-Objekts.|
|[Benutzer löschen](../api/intune_shared_user_delete.md).|Keine|Löscht einen [user](../resources/intune_shared_user.md).|
|[Update](../api/intune_shared_user_update.md) -Benutzerobjekt.|[user](../resources/intune_shared_user.md)|Aktualisieren der Eigenschaften eines [user](../resources/intune_shared_user.md)-Objekts.|
|**deviceManagement**|
|[removeAllDevicesFromManagement-Aktion](../api/intune_shared_user_removealldevicesfrommanagement.md)|Keine|Die Verwaltung aller Geräte für diesen Benutzer einstellen.|
|**Mobile app-Verwaltung (MAM)**|
|[getManagedAppDiagnosticStatuses-Funktion](../api/intune_shared_user_getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md)-Sammlung|Ruft den Status der Diagnoseüberprüfung für einen bestimmten Benutzer ab.|
|[getManagedAppPolicies-Funktion](../api/intune_shared_user_getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md)-Sammlung|Ruft App-Einschränkungen für einen bestimmten Benutzer ab.|
|[wipeManagedAppRegistrationsByDeviceTag-Aktion](../api/intune_shared_user_wipemanagedappregistrationsbydevicetag.md)|Keine|Gibt einen Zurücksetzungsvorgang für eine App-Registrierung mit angegebenem Geräte-Tag aus.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner des Benutzers|
|**Onboarding**|
|deviceEnrollmentLimit|Int32|Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann. Zulässige Werte sind 5 oder 1000.|


## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|**deviceManagement**|
|managedDevices|[managedDevice](../resources/intune_devices_manageddevice.md)-Sammlung|Die mit dem Benutzer verknüpften verwalteten Geräte.|
|**Mobile app-Verwaltung (MAM)**|
|managedAppRegistrations|[managedAppRegistration](../resources/intune_mam_managedappregistration.md)-Sammlung|Null oder mehr verwaltete App-Registrierungen, die dem Benutzer gehören.|
|**Problembehandlung**|
|deviceManagementTroubleshootingEvents|[deviceManagementTroubleshootingEvent](../resources/intune_troubleshooting_devicemanagementtroubleshootingevent.md)-Sammlung|Die Liste der Problembehandlungsereignisse für diesen Benutzer.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "@odata.type": "microsoft.graph.user"
}
--> 
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deviceEnrollmentLimit": 5
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: Resource microsoft.graph.user is defined in multiple files: /api-reference/v1.0/resources/intune_shared_user.md, /api-reference/v1.0/resources/user.md",
  ]
}-->
