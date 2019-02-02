---
title: Ressourcentyp relatedContact
description: Wenden Sie sich an Datensatz im Zusammenhang mit einer EducationUser, die Informationen für Aufsichtspersonen, Datenblätter, Ärzten und So weiter bereitstellt.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7e3829de2ffeb073d8360976ce70d13985fcae39
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694489"
---
# <a name="realtedcontact-resource-type"></a>Ressourcentyp realtedContact

Wenden Sie sich an Datensatz im Zusammenhang mit einer [EducationUser](../resources/educationuser.md) , die Informationen für Aufsichtspersonen, Datenblätter, Ärzten und So weiter bereitstellt.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|string|Die Identität des Kontakts in Azure Active Directory.|
|displayName|Zeichenfolge|Name des Kontakts. Erforderlich. |
|emailAddress|Zeichenfolge|Primäre e-Mail-Adresse des Kontakts.|
|mobilePhone|Zeichenfolge|Die Mobiltelefonnummer des Kontakts.|
|Beziehung|`contactRelationship`|Beziehung für den Benutzer. Mögliche Werte sind `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.|
|accessConsent|Boolescher Wert|Gibt an, ob der Benutzer Zugriff auf Daten Student zugestimmt wurde hat.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedContact"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "contactRelationship",
  "accessConsent": true
}
```

<!-- uuid: 720F9AB6-6E7A-4A66-8B0A-37A556FF99C5
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "relatedContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
