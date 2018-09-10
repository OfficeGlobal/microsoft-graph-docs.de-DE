# <a name="termsandconditionsacceptancestatus-resource-type"></a>termsAndConditionsAcceptanceStatus-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine termsAndConditionsAcceptanceStatus-Entität stellt den Annahmestatus einer bestimmten Geschäftsbedingungen-Richtlinie durch einen bestimmten Benutzer dar. Benutzer müssen die neueste Version der Geschäftsbedingungen akzeptieren, um weiterhin Zugriff auf das Unternehmensportal zu haben.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[termsAndConditionsAcceptanceStatuses auflisten](../api/intune_companyterms_termsandconditionsacceptancestatus_list.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)-Objekte.|
|[termsAndConditionsAcceptanceStatus abrufen](../api/intune_companyterms_termsandconditionsacceptancestatus_get.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|Lesen von Eigenschaften und Beziehungen des [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)-Objekts.|
|[termsAndConditionsAcceptanceStatus erstellen](../api/intune_companyterms_termsandconditionsacceptancestatus_create.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|Erstellen eines neuen [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)-Objekts.|
|[termsAndConditionsAcceptanceStatus löschen](../api/intune_companyterms_termsandconditionsacceptancestatus_delete.md)|Keine|Löscht ein [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)-Objekt.|
|[termsAndConditionsAcceptanceStatus aktualisieren](../api/intune_companyterms_termsandconditionsacceptancestatus_update.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|Aktualisieren der Eigenschaften eines [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|ID|Zeichenfolge|Eindeutiger Bezeichner der Entität|
|userDisplayName|String|Anzeigename des Benutzers, dessen Zustimmung die Entität darstellt|
|acceptedVersion|Int32|Die Versionsnummer der neuesten Version der Geschäftsbedingungen, die der Benutzer akzeptiert hat|
|acceptedDateTime|DateTimeOffset|Datum und Uhrzeit, zu der die Nutzungsbedingungen zuletzt vom Benutzer akzeptiert wurden.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Navigationslink zu den Geschäftsbedingungen, die zugewiesen werden.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```








