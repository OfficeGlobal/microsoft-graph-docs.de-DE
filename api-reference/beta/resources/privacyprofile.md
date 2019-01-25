---
title: privacyProfile-Ressourcentyp
description: Stellt das Datenschutzprofil eines Unternehmens dar, das eine URL zu einer Datenschutzerklärung sowie eine Kontaktperson für Fragen im Zusammenhang mit der Datenschutzerklärung umfasst.
localization_priority: Normal
ms.openlocfilehash: 9c110cbdb8a456b43936d3b56db5d4563686ed6e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510120"
---
# <a name="privacyprofile-resource-type"></a>privacyProfile-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt das Datenschutzprofil eines Unternehmens dar, das eine URL zu einer Datenschutzerklärung sowie eine Kontaktperson für Fragen im Zusammenhang mit der Datenschutzerklärung umfasst.

## <a name="properties"></a>Eigenschaften
| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|contactEmail|Zeichenfolge| Eine gültige SMTP-E-Mail-Adresse für den Kontakt für die Datenschutzerklärung Nicht erforderlich.|
|statementUrl|Zeichenfolge| Ein gültiges URL-Format, das mit „http://“ oder „https://“ beginnt. Die maximale Länge beträgt 255 Zeichen. Die URL, die zur Datenschutzerklärung des Unternehmens weiterleitet. Nicht erforderlich.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/privacyprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
