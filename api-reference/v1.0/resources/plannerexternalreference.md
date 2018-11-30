---
title: plannerExternalReference-Ressourcentyp
description: Die Ressource **PlannerExternalReference** stellt die Metadaten eines Verweises (Anlagen wie etwa URL-Datei). Es ist der Wert der Eigenschaft-Wert-Paare im ExternalReferences-Objekt.
ms.openlocfilehash: a9d53b487fd2ca6584af934c55388ee66b2071d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016412"
---
# <a name="plannerexternalreference-resource-type"></a>plannerExternalReference-Ressourcentyp

Die **plannerExternalReference**-Ressource stellt die Metadaten eines Verweises dar (Anlagen wie z. B. Datei, URL). Es ist der Wert von Eigenschaft-Wert-Paaren im [externalReferences](plannerexternalreferences.md)-Objekt.



## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|Alias|String|Ein Namensalias zur Beschreibung des Verweises.|
|lastModifiedBy|[identitySet](identityset.md)|Schreibgeschützt. Benutzer-ID, von der das Objekt zuletzt geändert wurde.|
|lastModifiedDateTime|DateTimeOffset|Schreibgeschützt. Datum und Uhrzeit der letzten Änderung des Objekts. Der Zeitstempeltyp stellt die Datums- und Uhrzeitinformationen im ISO 8601-Format dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|previewPriority|String|Wird verwendet, um die relative Prioritätsreihenfolge festzulegen, in der der Verweis als Vorschau für die Aufgaben angezeigt wirdd.|
|type|String|Wird verwendet, um den Verweis zu beschreiben. Zu den Typen gehören: `PowerPoint`, `Word`, `Excel`, `Other`.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->