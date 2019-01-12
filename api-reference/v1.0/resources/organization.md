---
title: organization-Ressourcentyp
description: " Erstellen und Delete werden nicht unterstützt. Erbt von directoryObject."
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c90299abeac92adcd8392b0058c94ba4e13ad2a1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912638"
---
# <a name="organization-resource-type"></a>organization-Ressourcentyp

Stellt dar, bei dem der Benutzer oder die Anwendung in angemeldet ist Azure Active Directory-Mandanten. Nur die Lese- und Aktualisierungsvorgänge werden für diese Ressource unterstützt. Erstellen und Delete werden nicht unterstützt. Erbt von [directoryObject](directoryobject.md).

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
| businessPhones                      | Zeichenfolgenauflistung                                         | Telefonnummer für die Organisation. Hinweis: Obgleich dies eine zeichenfolgenauflistung ist, kann nur eine Nummer für diese Eigenschaft festgelegt werden.                                                                                            |
| Ort                                 | Zeichenfolge                                                            | Der Name der Stadt aus der Unternehmensadresse                                                                                                                                                                                                                                        |
| Land                              | Zeichenfolge                                                            | Der Name des Landes/der Region aus der Unternehmensadresse                                                                                                                                                                                                                              |
| countryLetterCode                    | Zeichenfolge                                                            | Landes-/Regionsabkürzung für das Unternehmen                                                                                                                                                                                                                                     |
|createdDateTime|DateTimeOffset| Zeitstempel der Erstellung der Organisation. Der Wert kann nicht geändert werden und wird automatisch aufgefüllt, wenn die Organisation erstellt wird. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. |
| deletedDateTime                    | DateTimeOffset                                                    | Datum und Uhrzeit des darstellt, wenn es sich bei der Azure AD-Mandanten mit ISO 8601-Format gelöscht wurde, und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt.                                                                                     |
| displayName                          | Zeichenfolge                                                            | Der Anzeigename für den Mandanten.                                                                                                                                                                                                                                                     |
| id                                   | Zeichenfolge                                                            | Die Mandanten-ID eine eindeutige ID, die Organisation (oder des Mandanten) darstellt. Geerbt von [directoryObject](directoryobject.md). Schlüssel. Lässt keine Nullwerte zu. Schreibgeschützt.                                                                                                                                                            |
|isMultipleDataLocationsForServicesEnabled|Boolescher Wert|**true,** Wenn Organisation Multi-Geo aktiviert ist; **"false"** Wenn Organisation nicht aktiviert Multi-Geo. **null** (Standard). Schreibgeschützt. Weitere Informationen finden Sie unter [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
| marketingNotificationEmails          | Zeichenfolgenauflistung                                                 | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| onPremisesLastSyncDateTime               | DateTimeOffset                                                    | Uhrzeit und Datum der letzten Synchronisierung des Mandanten mit dem lokalen Verzeichnis. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. Schreibgeschützt. |
| onPremisesSyncEnabled                       | Boolean                                                           | **true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard).                        |
| postalCode                           | Zeichenfolge                                                            | Die Postleitzahl aus der Unternehmensadresse                                                                                                                                                                                                                                      |
| preferredLanguage                    | Zeichenfolge                                                            | Die bevorzugte Sprache für das Unternehmen. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en“.                                                                                                                                                                                         |
| privacyProfile                       | [privacyProfile](privacyprofile.md)                               | Das Datenschutzprofil einer Organisation.                                                                                                                                                                                                                                              |
| provisionedPlans                     | [ProvisionedPlan-Sammlung](provisionedplan.md)                  | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
| securityComplianceNotificationMails  | Zeichenfolgenauflistung                                                 |                                                                                                                                                                                                                                                                                      |
| securityComplianceNotificationPhones | Zeichenfolgenauflistung                                                 |                                                                                                                                                                                                                                                                                      |
| state                                | Zeichenfolge                                                            | Der das Bundesland aus der Unternehmensadresse                                                                                                                                                                                                                                       |
| street                               | Zeichenfolge                                                            | Der Straßenname aus der Unternehmensadresse                                                                                                                                                                                                                                          |
| technicalNotificationMails           | Zeichenfolgenauflistung                                                 | Lässt keine Nullwerte zu.                                                                                                                                                                                                                                                                        |
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

## <a name="see-also"></a>Weitere Artikel

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
