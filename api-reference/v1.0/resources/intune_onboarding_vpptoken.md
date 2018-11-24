# <a name="vpptoken-resource-type"></a>vppToken-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Sie erwerben mehrere Lizenzen für iOS-Apps über das Apple Volume Purchase Program for Business oder Education. Dies umfasst das Einrichten eines Apple VPP-Kontos auf der Apple-Website und das Hochladen des Apple VPP Business- oder Education-Tokens in Intune. Dann können Sie Ihre Volumenlizenzierungsinformationen mit Intune synchronisieren und die volumenlizenzierte App-Nutzung nachverfolgen. Sie können mehrere Apple VPP Business- oder Education-Token hochladen.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[VppTokens auflisten](../api/intune_onboarding_vpptoken_list.md)|[VppToken](../resources/intune_onboarding_vpptoken.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [vppToken](../resources/intune_onboarding_vpptoken.md)-Objekte.|
|[VppToken abrufen](../api/intune_onboarding_vpptoken_get.md)|[vppToken](../resources/intune_onboarding_vpptoken.md)|Lesen von Eigenschaften und Beziehungen des [vppToken](../resources/intune_onboarding_vpptoken.md)-Objekts.|
|[VppToken erstellen](../api/intune_onboarding_vpptoken_create.md)|[vppToken](../resources/intune_onboarding_vpptoken.md)|Erstellen eines neuen [vppToken](../resources/intune_onboarding_vpptoken.md)-Objekts.|
|[VppToken löschen](../api/intune_onboarding_vpptoken_delete.md)|Keine|Löscht ein [vppToken](../resources/intune_onboarding_vpptoken.md).|
|[VppToken aktualisieren](../api/intune_onboarding_vpptoken_update.md)|[vppToken](../resources/intune_onboarding_vpptoken.md)|Aktualisieren der Eigenschaften eines [vppToken](../resources/intune_onboarding_vpptoken.md)-Objekts.|
|[syncLicenses-Aktion](../api/intune_onboarding_vpptoken_synclicenses.md)|[vppToken](../resources/intune_onboarding_vpptoken.md)|Synchronisiert Lizenzen, die einem bestimmten appleVolumePurchaseProgramToken zugeordnet sind|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Dies wird automatisch generiert, wenn das appleVolumePurchaseProgramToken erstellt wird. Es ist der Schlüssel für die Entität.|
|organizationName|String|Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune_shared_vpptokenaccounttype.md)|Volume Purchase Program-Typ, dem das angegebene Apple Volume Purchase Program-Token zugeordnet ist. Mögliche Werte sind: `business` und `education`. Mögliche Werte sind: `business` und `education`.|
|appleId|String|Die Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist.|
|expirationDateTime|DateTimeOffset|Ablaufdatum und -Uhrzeit des Apple Volume Purchase Program-Tokens|
|lastSyncDateTime|DateTimeOffset|Der Zeitpunkt der letzten Anwendungssynchronisierung mit dem Apple Volume Purchase Program-Dienst mithilfe des Apple Volume Purchase Program-Tokens.|
|token|String|Die Zeichenfolge des Apple Volume Purchase Program-Tokens, die vom Apple Volume Purchase Program heruntergeladen wurde.|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung, die dem Apple Volume Purchase Program-Token zugeordnet sind.|
|state|[vppTokenState](../resources/intune_onboarding_vpptokenstate.md)|Aktueller Status des Apple Volume Purchase Program-Tokens. Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid` und `assignedToExternalMDM`. Mögliche Werte sind: `unknown`, `valid`, `expired`, `invalid` und `assignedToExternalMDM`.|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune_onboarding_vpptokensyncstatus.md)|Aktueller Synchronisierungsstatus der letzten Anwendungssynchronisierung, die mit dem Apple Volume Purchase Program-Token ausgelöst wurde. Mögliche Werte sind: `none`, `inProgress`, `completed` und `failed`. Mögliche Werte sind: `none`, `inProgress`, `completed` und `failed`.|
|automaticallyUpdateApps|Boolean|Gibt an, ob Apps für das VPP-Token automatisch aktualisiert werden.|
|countryOrRegion|String|Gibt an, ob Apps für das VPP-Token automatisch aktualisiert werden.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppToken"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "String (identifier)",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String"
}
```



