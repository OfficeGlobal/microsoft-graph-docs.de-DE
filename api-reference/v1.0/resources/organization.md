# <a name="organization-resource-type"></a>organization-Ressourcentyp

Stellt einen Azure Active Directory-Mandanten dar. Für Mandanten werden nur Lese- und Aktualisierungsvorgänge unterstützt. Erstellen und Löschen werden nicht unterstützt. Erbt von [directoryObject](directoryobject.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[organization abrufen](../api/organization_get.md) | [organization](organization.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des organization-Objekts.|
|[Update](../api/organization_update.md) | [organization](organization.md)  |Dient zum Aktualisieren des organization-Objekts. (Nur die **marketingNotificationMails**- und die **technicalNotificationMails**-Eigenschaft kann aktualisiert werden.) |

## <a name="properties"></a>Eigenschaften

| Eigenschaft                             | Typ                                                              | Beschreibung                                                                                                                                                                                                                                                                          |
|:-------------------------------------|:------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| assignedPlans                        | [assignedPlan](assignedplan.md)-Sammlung                        | Die Sammlung von Serviceplänen, die dem Mandanten zugeordnet sind. Lässt keine Nullwerte zu.                                                                                                                                                                                                            |
| Ort                                 | String                                                            |                                                                                                                                                                                                                                                                                      |
| companyLastDirSyncTime               | DateTimeOffset                                                    | Zeit und Datum der letzten Synchronisierung des Mandanten mit dem lokalen Verzeichnis. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'` |
| Land                              | String                                                            |                                                                                                                                                                                                                                                                                      |
| countryLetterCode                    | String                                                            |                                                                                                                                                                                                                                                                                      |
| deletionTimestamp                    | DateTimeOffset                                                    | Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`                                                                                     |
| dirSyncEnabled                       | Boolean                                                           | **true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard).                        |
| displayName                          | String                                                            | Der Anzeigename für den Mandanten.                                                                                                                                                                                                                                                     |
| id                                   | String                                                            | Der eindeutige Bezeichner für den Mandanten. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.                                                                                                                                                            |
| marketingNotificationEmails          | String collection                                                 | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| objectType                           | String                                                            | Eine Zeichenfolge, die den Objekttyp identifiziert. Für Mandanten ist der Wert immer „Unternehmen“.                                                                                                                                                                                                 |
| postalCode                           | String                                                            |                                                                                                                                                                                                                                                                                      |
| preferredLanguage                    | String                                                            |                                                                                                                                                                                                                                                                                      |
| provisionedPlans                     | [ProvisionedPlan-Sammlung](provisionedplan.md)                  | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| provisioningErrors                   | ProvisioningError-Sammlung | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| securityComplianceNotificationMails  | String collection                                                 |                                                                                                                                                                                                                                                                                      |
| securityComplianceNotificationPhones | String collection                                                 |                                                                                                                                                                                                                                                                                      |
| state                                | String                                                            |                                                                                                                                                                                                                                                                                      |
| street                               | String                                                            |                                                                                                                                                                                                                                                                                      |
| technicalNotificationMails           | String collection                                                 | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| telephoneNumber                      | String                                                            |                                                                                                                                                                                                                                                                                      |
| verifiedDomains                      | [VerifiedDomain-Sammlung](verifieddomain.md)                    | Die Sammlung von Domänen, die diesem Mandanten zugeordnet sind. Lässt keine Nullwerte zu.                                                                                                                                                                                                                 |

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
