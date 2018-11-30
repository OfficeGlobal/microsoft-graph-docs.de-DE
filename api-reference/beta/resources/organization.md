---
title: organization-Ressourcentyp
description: 'Stellt eine Azure Active Directory-Mandanten. '
ms.openlocfilehash: 0dc7b55053ba70272c4e639dba4b62160f58f435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060810"
---
# <a name="organization-resource-type"></a>organization-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Azure Active Directory-Mandanten. 

Diese Ressource ermöglicht es Ihnen, benutzerdefinierten Eigenschaften mithilfe von [Erweiterungen](/graph/extensibility-overview) eigene Daten hinzuzufügen.

Nur die Lese- und Aktualisierungsvorgänge werden auf Mandanten unterstützt. Erstellen und Delete werden nicht unterstützt. Erbt von [directoryObject](directoryobject.md).

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[organization abrufen](../api/organization-get.md) | [organization](organization.md) |Dient zum Lesen der Eigenschaften und der Beziehungen des organization-Objekts.|
|[Update](../api/organization-update.md) | [organization](organization.md)  |Dient zum Aktualisieren des organization-Objekts. Die einzigen Eigenschaften, die aktualisiert werden können, sind: **marketingNotificationMails**, **technicalNotificationMails**, **securityComplianceNotificationMails**, **securityComplianceNotificationPhones** und **privacyProfile**. |
|**Offene Erweiterungen**| | |
|[Offene Erweiterung erstellen](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Erstellt eine offene Erweiterung und fügt benutzerdefinierte Eigenschaften zu einer neuen oder vorhandenen Ressource hinzu.|
|[Offene Erweiterung abrufen](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md)-Sammlung| Dient zum Abrufen einer offenen Erweiterung, die durch den Erweiterungsnamen identifiziert wird.|
|**Schemaerweiterungen**| | |
|[Schemaerweiterungswerte hinzufügen](/graph/extensibility-schema-groups) || Dient zum Erstellen einer Schemaerweiterungsdefinition und anschließenden Verwenden der Definition zum Hinzufügen benutzerdefinierter typisierter Daten zu einer Ressource.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assignedPlans|[assignedPlan](assignedplan.md)-Sammlung|Die Sammlung von Serviceplänen, die dem Mandanten zugeordnet sind. Lässt keine Nullwerte zu.            |
|Ort|Zeichenfolge| Der Name der Stadt aus der Unternehmensadresse |
|companyLastDirSyncTime|DateTimeOffset|Zeit und Datum der letzten Synchronisierung des Mandanten mit dem lokalen Verzeichnis. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|Land|Zeichenfolge| Der Name des Landes/der Region aus der Unternehmensadresse |
|countryLetterCode|Zeichenfolge| Landes-/Regionsabkürzung für das Unternehmen |
|deletionTimestamp|DateTimeOffset|Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|dirSyncEnabled|Boolean|**true**, wenn das Objekt aus einem lokalen Verzeichnis synchronisiert wird; **false**, wenn das Objekt ursprünglich aus einem lokalen Verzeichnis synchronisiert wurde, aber nicht mehr synchronisiert wird; **NULL**, wenn dieses Objekt nie aus einem lokalen Verzeichnis synchronisiert wurde (Standard).|
|displayName|String|Der Anzeigename für den Mandanten.|
|id|String|Der eindeutige Bezeichner für den Mandanten. Geerbt von [directoryObject](directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt.|
|isMultipleDataLocationsForServicesEnabled|Boolesch|**true,** Wenn Organisation Multi-Geo aktiviert ist; **"false"** Wenn Organisation nicht aktiviert Multi-Geo. **null** (Standard). Schreibgeschützt. Weitere Informationen finden Sie unter [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|marketingNotificationEmails|Zeichenfolgenauflistung| Lässt keine Nullwerte zu.            |
|objectType|String|Eine Zeichenfolge, die den Objekttyp identifiziert. Für Mandanten ist der Wert immer „Unternehmen“. |
|postalCode|Zeichenfolge| Die Postleitzahl aus der Unternehmensadresse |
|preferredLanguage|Zeichenfolge| Die bevorzugte Sprache für das Unternehmen. Muss im ISO 639-1-Code angegeben werden. Beispiel: „en“. |
|privacyProfile|[privacyProfile](privacyprofile.md)| Das Datenschutzprofil einer Organisation.            |
|provisionedPlans|[ProvisionedPlan-Sammlung](provisionedplan.md)| Lässt keine Nullwerte zu.            |
|provisioningErrors|ProvisioningError-Sammlung| Lässt keine Nullwerte zu.            |
|securityComplianceNotificationMails|Zeichenfolgenauflistung||
|securityComplianceNotificationPhones|Zeichenfolgenauflistung||
|state|Zeichenfolge| Der das Bundesland aus der Unternehmensadresse |
|street|Zeichenfolge| Der Straßenname aus der Unternehmensadresse |
|technicalNotificationMails|Zeichenfolgenauflistung| Lässt keine Nullwerte zu. |
|telephoneNumber|Zeichenfolge| Die Telefonnummer des Unternehmens |
|verifiedDomains|[VerifiedDomain-Sammlung](verifieddomain.md)|Die Sammlung von Domänen, die diesem Mandanten zugeordnet sind. Lässt keine Nullwerte zu.            |

## <a name="relationships"></a>Beziehungen
| Erweiterungen | [Erweiterung](extension.md) -Auflistung | Die Auflistung der open-Erweiterungen für die Ressource für die Organisation definiert. NULL-Werte zulässt. |

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
  "tocPath": ""
}-->
