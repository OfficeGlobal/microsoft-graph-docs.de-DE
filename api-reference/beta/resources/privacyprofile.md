---
title: privacyProfile-Ressourcentyp
description: Stellt das Datenschutzprofil eines Unternehmens dar, das eine URL zu einer Datenschutzerklärung sowie eine Kontaktperson für Fragen im Zusammenhang mit der Datenschutzerklärung umfasst.
ms.openlocfilehash: fb9d5f929f1c9ae28687b80e987dc0909387f5d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065766"
---
# <a name="privacyprofile-resource-type"></a>privacyProfile-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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