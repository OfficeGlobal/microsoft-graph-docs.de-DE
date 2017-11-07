# <a name="organization-resource-type"></a>organization-Ressourcentyp

Stellt einen Azure Active Directory-Mandanten dar. Für Mandanten werden nur Lese- und Aktualisierungsvorgänge unterstützt. Erstellen und Löschen werden nicht unterstützt. Erbt von [directoryObject](directoryobject.md).

Diese Ressource ermöglicht es Ihnen, benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](../../../concepts/extensibility_overview.md) eigene Daten hinzuzufügen.


## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[organization abrufen](../api/organization_get.md) | [organization](organization.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des organization-Objekts.|
|[Update](../api/organization_update.md) | [organization](organization.md)  |Dient zum Aktualisieren des organization-Objekts. (Nur die **marketingNotificationMails**- und die **technicalNotificationMails**-Eigenschaft kann aktualisiert werden.) |
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](../../../concepts/extensibility_schema_groups.md) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft                             | Typ                                                              | Beschreibung                                                                                                                                                                                                                                                                          |
|:-------------------------------------|:------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| assignedPlans                        | [assignedPlan](assignedplan.md)-Sammlung                        | Die Sammlung von Serviceplänen, die dem Mandanten zugeordnet sind. Lässt keine Nullwerte zu.                                                                                                                                                                                                            |
| Ort                                 | Zeichenfolge                                                            | Der Name der Stadt aus der Unternehmensadresse                                                                                                                                                                                                                                        |
| companyLastDirSyncTime               | DateTimeOffset                                                    | Zeit und Datum der letzten Synchronisierung des Mandanten mit dem lokalen Verzeichnis. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'` |
| Land                              | Zeichenfolge                                                            | Der Name des Landes/der Region aus der Unternehmensadresse                                                                                                                                                                                                                                     |
| countryLetterCode                    | Zeichenfolge                                                            | Landes-/Regionsabkürzung für das Unternehmen                                                                                                                                                                                                                                            |
| deletionTimestamp                    | DateTimeOffset                                                    | Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`                                                                                     |
| dirSyncEnabled                       | Boolean                                                           | **true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard).                        |
| displayName                          | String                                                            | Der Anzeigename für den Mandanten.                                                                                                                                                                                                                                                     |
| id                                   | String                                                            | Der eindeutige Bezeichner für den Mandanten. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.                                                                                                                                                            |
| marketingNotificationEmails          | String collection                                                 | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| objectType                           | String                                                            | Eine Zeichenfolge, die den Objekttyp identifiziert. Für Mandanten ist der Wert immer „Unternehmen“.                                                                                                                                                                                                 |
| postalCode                           | Zeichenfolge                                                            | Die Postleitzahl aus der Unternehmensadresse                                                                                                                                                                                                                                      |
| preferredLanguage                    | Zeichenfolge                                                            | Die bevorzugte Sprache für das Unternehmen. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en“.                                                                                                                                                                                         |
| provisionedPlans                     | [ProvisionedPlan-Sammlung](provisionedplan.md)                  | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| provisioningErrors                   | ProvisioningError-Sammlung                                      | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| securityComplianceNotificationMails  | String collection                                                 |                                                                                                                                                                                                                                                                                      |
| securityComplianceNotificationPhones | String collection                                                 |                                                                                                                                                                                                                                                                                      |
| state                                | Zeichenfolge                                                            | Der das Bundesland aus der Unternehmensadresse                                                                                                                                                                                                                                       |
| street                               | Zeichenfolge                                                            | Der Straßenname aus der Unternehmensadresse                                                                                                                                                                                                                                          |
| technicalNotificationMails           | String collection                                                 | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| telephoneNumber                      | Zeichenfolge                                                            | Die Telefonnummer des Unternehmens                                                                                                                                                                                                                                                |
| verifiedDomains                      | [VerifiedDomain-Sammlung](verifieddomain.md)                    | Die Sammlung von Domänen, die diesem Mandanten zugeordnet sind. Lässt keine Nullwerte zu.                                                                                                                                                                                                                 |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Sammlung der für die Organisation definierten offenen Erweiterungen. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["string"],
  "city": "string",
  "country": "string",
  "countryLetterCode": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "marketingNotificationEmails": ["string"],
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}

```

## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](../../../concepts/extensibility_overview.md)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](../../../concepts/extensibility_open_users.md)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
