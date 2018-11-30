---
title: Ressourcentyp educationFileResource
description: Eine Unterklasse der EducationResource, die ein File-Objekt darstellt, die die Zuordnung oder die Übermittlung zugeordnet ist.  In diesem Fall wird die Datei ist nicht die speziellen Dateien (Word, Excel usw.), jedoch ist eine Datei, die keine besondere Behandlung innerhalb des Systems verfügt. File-Ressource muss in der **Ressourcefolder** gespeichert werden, die die Zuordnung oder die Übermittlung, diese Ressource zugeordnet ist, zugeordnet ist.
ms.openlocfilehash: b3ba77b6b9243d987ad1137afe6d2206e47dadaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062217"
---
# <a name="educationfileresource-resource-type"></a>Ressourcentyp educationFileResource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine Unterklasse der [EducationResource](educationresource.md) , die ein File-Objekt darstellt, die die Zuordnung oder die Übermittlung zugeordnet ist.  In diesem Fall wird die Datei ist nicht die speziellen Dateien (Word, Excel usw.), jedoch ist eine Datei, die keine besondere Behandlung innerhalb des Systems verfügt. File-Ressource muss in der **Ressourcefolder** gespeichert werden, die die Zuordnung oder die Übermittlung, diese Ressource zugeordnet ist, zugeordnet ist.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|fileUrl|String|Speicherort auf dem Datenträger den File-Ressource.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->