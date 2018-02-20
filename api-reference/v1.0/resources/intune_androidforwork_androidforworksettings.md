# <a name="androidforworksettings-resource-type"></a>Ressourcentyp „androidForWorkSettings“

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Einstellungen für Android for Work
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von „androidForWorkSettings“](../api/intune_androidforwork_androidforworksettings_get.md)|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|Liest Eigenschaften und Beziehungen des Objekts [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md).|
|[Aktualisieren von „androidForWorkSettings“](../api/intune_androidforwork_androidforworksettings_update.md)|[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md)|Aktualisiert die Eigenschaften eines Objekts des Typs [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md).|
|[Aktion „requestSignupUrl“](../api/intune_androidforwork_androidforworksettings_requestsignupurl.md)|String|Generiert eine Registrierungs-URL, die zur Registrierung in der Android for Work-Verwaltung verwendet wird.|
|[Aktion „completeSignup“](../api/intune_androidforwork_androidforworksettings_completesignup.md)|Keiner|Schließt den Fluss zur Registrierung in der Android for Work-Verwaltung ab.|
|[Aktion „syncApps“](../api/intune_androidforwork_androidforworksettings_syncapps.md)|Keiner|Synchronisiert genehmigte Anwendungen für das Unternehmen.|
|[Aktion „unbind“](../api/intune_androidforwork_androidforworksettings_unbind.md)|Keiner|Deaktiviert die Android for Work-Verwaltung für das Unternehmen.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Android for Work-Einstellungsbezeichner|
|bindStatus|String|Status der Bindung des Mandanten mit der EMM-API von Google. Mögliche Werte sind: `notBound`, `bound`, `boundAndValidated` und `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Zeitpunkt, zu dem zuletzt eine App-Synchronisierung abgeschlossen wurde|
|lastAppSyncStatus|String|Ergebnis der letzten Anwendungssynchronisierung. Mögliche Werte sind: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError` und `none`.|
|ownerUserPrincipalName|String|Besitzer-UPN, der das Unternehmen erstellt hat|
|ownerOrganizationName|String|Organisationsname, der beim Android for Work-Onboarding verwendet wird|
|lastModifiedDateTime|DateTimeOffset|Zeitpunkt, zu dem die Android for Work-Einstellungen zuletzt geändert wurden|
|enrollmentTarget|String|Gibt an, welche Benutzer Geräte in der Android for Work-Geräteverwaltung registrieren dürfen. Mögliche Werte sind: `none`, `all`, `targeted` und `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|String-Sammlung|Gibt an, welche AAD-Gruppen Geräte in der Android for Work-Geräteverwaltung registrieren dürfen, wenn die Eigenschaft „enrollmentTarget“ auf „Targeted“ gesetzt ist.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Unten sehen Sie eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ]
}
```



