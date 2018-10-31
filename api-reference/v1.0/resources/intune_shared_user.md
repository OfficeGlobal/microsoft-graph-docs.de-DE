# <a name="user-resource-type"></a>user-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt ein user-Objekt von Azure Active Directory dar.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Benutzer auflisten](../api/intune_shared_user_list.md)-Objekte.|[user](../resources/intune_shared_user.md)-sammlung|Auflisten von Eigenschaften und Beziehungen der [Benutzer](../resources/intune_shared_user.md)-Objekte.|
|[Benutzer abrufen](../api/intune_shared_user_get.md)-Objekt.|[user](../resources/intune_shared_user.md)-sammlung|Lesen von Eigenschaften und Beziehungen des [Benutzer](../resources/intune_shared_user.md)-Objekts.|
|[Benutzer erstellen](../api/intune_shared_user_create.md)-Objekt.|[user](../resources/intune_shared_user.md)-sammlung|Dient zum Erstellen eines neuen [Benutzer](../resources/intune_shared_user.md)-Objekts.|
|[Benutzer löschen](../api/intune_shared_user_delete.md).|Keine|Löscht ein [user](../resources/intune_shared_user.md)-Objekt.|
|[Benutzer aktualisieren](../api/intune_shared_user_update.md)-Objekt.|[Benutzer](../resources/intune_shared_user.md)|Aktualisieren der Eigenschaften eines [Benutzer](../resources/intune_shared_user.md)-Objekts.|
|**Geräteverwaltung**|
|[removeAllDevicesFromManagement-Aktion](../api/intune_shared_user_removealldevicesfrommanagement.md)|Keine|Die Verwaltung aller Geräte für diesen Benutzer einstellen.|
|**Mobile Anwendungsverwaltung (MAM)**|
|[getManagedAppDiagnosticStatuses-Funktion](../api/intune_shared_user_getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md)-Sammlung|Ruft den Status der Diagnoseüberprüfung für einen bestimmten Benutzer ab.|
|[getManagedAppPolicies-Funktion](../api/intune_shared_user_getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md)-Sammlung|Ruft App-Einschränkungen für einen bestimmten Benutzer ab.|
|[wipeManagedAppRegistrationsByDeviceTag-Aktion](../api/intune_shared_user_wipemanagedappregistrationsbydevicetag.md)|Keine|Gibt einen Zurücksetzungsvorgang für eine App-Registrierung mit angegebenem Geräte-Tag aus.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Eindeutiger Bezeichner des Benutzers|
|**Onboarding**|
|deviceEnrollmentLimit|Int32|Der Grenzwert für die maximale Anzahl von Geräten, die der Benutzer registrieren kann. Zulässige Werte sind 5 oder 1000.|


## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|**Geräteverwaltung**|
|managedDevices|[managedDevice](../resources/intune_devices_manageddevice.md)-Sammlung|Die dem Benutzer zugeordneten verwalteten Geräte.|
|**Mobile Anwendungsverwaltung (MAM)**|
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
