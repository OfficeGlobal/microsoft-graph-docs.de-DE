---
title: organization-Ressourcentyp
description: " Erstellen und Löschen werden nicht unterstützt. Erbt von directoryObject."
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ecd92005849870704002c4e7617d2f0e76a7031b
ms.sourcegitcommit: 7412dd2f2d5ed66afa2b0759c861ad23b4c6ecdf
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/23/2019
ms.locfileid: "30212368"
---
# <a name="organization-resource-type"></a>organization-Ressourcentyp

Steht für den Azure Active Directory-Mandanten, bei dem der Benutzer oder die Anwendung angemeldet ist. Für diese Ressource werden nur Lese- und Aktualisierungsvorgänge unterstützt. Erstellen und Löschen werden nicht unterstützt. Erbt von [directoryObject](directoryobject.md).

Diese Ressource ermöglicht es Ihnen, benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](/graph/extensibility-overview) eigene Daten hinzuzufügen.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[organization abrufen](../api/organization-get.md) | [organization](organization.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des organization-Objekts.|
|[Update](../api/organization-update.md) | [organization](organization.md)  |Dient zum Aktualisieren des organization-Objekts. Die einzigen Eigenschaften, die aktualisiert werden können, sind: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** und **privacyProfile**. |
|**Offene Erweiterungen**| 
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| 
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft                             | Typ                                                              | Beschreibung                                                                                                                                                                                                                                                                          |
|:-------------------------------------|:------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| assignedPlans                        | [assignedPlan](assignedplan.md)-Sammlung                        | Die Sammlung von Serviceplänen, die dem Mandanten zugeordnet sind. Lässt keine Nullwerte zu.                                                                                                                                                                                                            |
| businessPhones                      | String-Sammlung                                         | Telefonnummer des Unternehmens. HINWEIS: Obwohl dies eine String-Sammlung ist, kann nur eine Nummer für diese Eigenschaft festgelegt werden.                                                                                            |
| city                                 | Zeichenfolge                                                            | Name der Stadt aus der Unternehmensadresse                                                                                                                                                                                                                                        |
| country                              | Zeichenfolge                                                            | Der Name des Landes/der Region aus der Unternehmensadresse                                                                                                                                                                                                                              |
| countryLetterCode                    | Zeichenfolge                                                            | Landes-/Regionsabkürzung für das Unternehmen                                                                                                                                                                                                                                     |
|createdDateTime|DateTimeOffset| Zeitstempel der Erstellung der Organisation. Der Wert kann nicht geändert werden und wird automatisch ausgefüllt, wenn die Organisation erstellt wird. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. |
| deletedDateTime                    | DateTimeOffset                                                    | Gibt Datum und Uhrzeit der Löschung des Azure AD-Mandanten an. ISO 8601-Format, immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.                                                                                     |
|createdDateTime|DateTimeOffset| Zeitstempel der Erstellung der Organisation. Der Wert kann nicht geändert werden und wird automatisch ausgefüllt, wenn die Organisation erstellt wird. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. |
| displayName                          | String                                                            | Der Anzeigename für den Mandanten.                                                                                                                                                                                                                                                     |
| id                                   | String                                                            | Mandanten-ID, ein eindeutiger Bezeichner, der für die Organisation (oder den Mandanten) steht. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.                                                                                                                                                            |
|isMultipleDataLocationsForServicesEnabled|Boolean|**true**, wenn die Organisation Multi-Geo-fähig ist; **false**, wenn die Organisation nicht Multi-Geo-fähig ist; **null** (Standard). Schreibgeschützt. Weitere Informationen finden Sie unter [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
| marketingNotificationEmails          | String collection                                                 | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| onPremisesLastSyncDateTime               | DateTimeOffset                                                    | Uhrzeit und Datum der letzten Synchronisierung des Mandanten mit dem lokalen Verzeichnis. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. |
| onPremisesSyncEnabled                       | Boolean                                                           | **true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard).                        |
| postalCode                           | Zeichenfolge                                                            | Die Postleitzahl aus der Unternehmensadresse                                                                                                                                                                                                                                      |
| preferredLanguage                    | Zeichenfolge                                                            | Die bevorzugte Sprache für das Unternehmen. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en“.                                                                                                                                                                                         |
| privacyProfile                       | [privacyProfile](privacyprofile.md)                               | Das Datenschutzprofil einer Organisation.                                                                                                                                                                                                                                              |
| provisionedPlans                     | [ProvisionedPlan-Sammlung](provisionedplan.md)                  | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| securityComplianceNotificationMails  | String collection                                                 |                                                                                                                                                                                                                                                                                      |
| securityComplianceNotificationPhones | String collection                                                 |                                                                                                                                                                                                                                                                                      |
| state                                | Zeichenfolge                                                            | Der das Bundesland aus der Unternehmensadresse                                                                                                                                                                                                                                       |
| street                               | Zeichenfolge                                                            | Der Straßenname aus der Unternehmensadresse                                                                                                                                                                                                                                          |
| technicalNotificationMails           | String collection                                                 | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| verifiedDomains                      | [VerifiedDomain-Sammlung](verifieddomain.md)                    | Die Sammlung von Domänen, die diesem Mandanten zugeordnet sind. Lässt keine Nullwerte zu.                                                                                                                                                                                                                 |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Erweiterungen|[extension](extension.md)-Sammlung|Die Sammlung der für die Organisation definierten offenen Erweiterungen. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "extensions"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.organization"
}-->

```json
{
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "businessPhones": ["string"],
  "city": "string",
  "country": "string",
  "countryLetterCode": "string",
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "string",
  "id": "string (identifier)",
  "isMultipleDataLocationsForServicesEnabled": "boolean",
  "marketingNotificationEmails": ["string"],
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "preferredLanguage": "string",
  "privacyProfile": {"@odata.type": "microsoft.graph.privacyProfile"},
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "securityComplianceNotificationMails": ["string"],
  "securityComplianceNotificationPhones": ["string"],
  "state": "string",
  "street": "string",
  "technicalNotificationMails": ["string"],
  "verifiedDomains": [{"@odata.type": "microsoft.graph.verifiedDomain"}]
}
```

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen](/graph/extensibility-open-users)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organization resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'businessPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesLastSyncDateTime' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'onPremisesSyncEnabled' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationMails' found in resource definition for 'microsoft.graph.organization', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/organization.md:
      Property 'securityComplianceNotificationPhones' found in resource definition for 'microsoft.graph.organization', but not described in markdown table."
  ],
  "tocPath": ""
}-->
