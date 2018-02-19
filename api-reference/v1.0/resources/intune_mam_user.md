# <a name="user-resource-type"></a>user-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Stellt ein user-Objekt von Azure Active Directory dar.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Benutzer auflisten](../api/intune_mam_user_list.md)|[user](../resources/intune_mam_user.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [user](../resources/intune_mam_user.md)-Objekte.|
|[Benutzer abrufen](../api/intune_mam_user_get.md)|[user](../resources/intune_mam_user.md)|Lesen von Eigenschaften und Beziehungen des [user](../resources/intune_mam_user.md)-Objekts.|
|[Benutzer erstellen](../api/intune_mam_user_create.md)|[user](../resources/intune_mam_user.md)|Erstellen eines neuen [user](../resources/intune_mam_user.md)-Objekts.|
|[Benutzer löschen](../api/intune_mam_user_delete.md)|Keine|Löscht ein [user](../resources/intune_mam_user.md)-Objekt.|
|[Benutzer aktualisieren](../api/intune_mam_user_update.md)|[user](../resources/intune_mam_user.md)|Aktualisieren der Eigenschaften eines [user](../resources/intune_mam_user.md)-Objekts.|
|[getManagedAppDiagnosticStatuses-Funktion](../api/intune_mam_user_getmanagedappdiagnosticstatuses.md)|[managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md)-Sammlung|Ruft den Status der Diagnoseüberprüfung für einen bestimmten Benutzer ab.|
|[getManagedAppPolicies-Funktion](../api/intune_mam_user_getmanagedapppolicies.md)|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md)-Sammlung|Ruft App-Einschränkungen für einen bestimmten Benutzer ab.|
|[wipeManagedAppRegistrationsByDeviceTag-Aktion](../api/intune_mam_user_wipemanagedappregistrationsbydevicetag.md)|Keine|Gibt einen Zurücksetzungsvorgang für eine App-Registrierung mit angegebenem Geräte-Tag aus.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Der Benutzerbezeichner.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managedAppRegistrations|[managedAppRegistration](../resources/intune_mam_managedappregistration.md)-Sammlung|Null oder mehr verwaltete App-Registrierungen, die dem Benutzer gehören.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



