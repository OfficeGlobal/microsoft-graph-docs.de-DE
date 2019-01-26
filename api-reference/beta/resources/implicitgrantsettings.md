---
title: Ressourcentyp implicitGrantSettings
description: Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann. Separate Eigenschaften sind verfügbar als Teil der implizite Ablauf Token-ID und Zugriff anfordern. Um implizite Ablauf aktivieren, mindestens eine der folgenden Eigenschaften festgelegt werden muss auf "true".
localization_priority: Normal
ms.openlocfilehash: 82051c3605d9815fef8a0852e0ffa9075f4a6d78
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574516"
---
# <a name="implicitgrantsettings-resource-type"></a>Ressourcentyp implicitGrantSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Gibt an, ob dieser Webanwendung mithilfe des impliziten OAuth 2.0-Fluss Token angefordert werden kann. Separate Eigenschaften sind verfügbar als Teil der implizite Ablauf Token-ID und Zugriff anfordern. Um implizite Ablauf aktivieren, mindestens eine der folgenden Eigenschaften festgelegt werden muss auf "true".

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------|:-----|:------------|
|enableIdTokenIssuance| Boolean | Gibt an, ob diese Web Application ein Token-ID mithilfe des impliziten OAuth 2.0-Fluss anfordern kann.|
|enableAccessTokenIssuance| Boolean | Gibt an, ob diese Web Application ein Zugriffstoken mit den impliziten OAuth 2.0-Fluss anfordern kann.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.implicitGrantSettings"
}-->
```json
{
  "enableIdTokenIssuance": "Boolean",
  "enableAccessTokenIssuance": "Boolean"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/implicitgrantsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
