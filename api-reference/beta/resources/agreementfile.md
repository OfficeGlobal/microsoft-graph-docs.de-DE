---
title: Ressourcentyp agreementFile
description: Stellt eine anpassbare Begriffe der Vereinbarung-Datei verwenden, die ein Mandanten mit Azure Active Directory (AD Azure) verwaltet. Es enthält Metadaten zu einer Datei Vereinbarung (beispielsweise den Namen, die Sprache und ob sie die Standarddatei ist).
ms.openlocfilehash: f099715fd25fbae9d7b2a94d6de841b8766c30e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061945"
---
# <a name="agreementfile-resource-type"></a>Ressourcentyp agreementFile

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine anpassbare Begriffe der Vereinbarung-Datei verwenden, die ein Mandanten mit Azure Active Directory (AD Azure) verwaltet. Es enthält Metadaten zu einer Datei Vereinbarung (beispielsweise den Namen, die Sprache und ob sie die Standarddatei ist).

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|fileData|[agreementFileData](agreementfiledata.md)|Daten, die die Begriffe verwenden PDF-Dokument darstellt. Schreibgeschützt.|
|fileName|String|Name der Datei Vereinbarung (beispielsweise TOU.pdf). Schreibgeschützt.|
|id|String|Schreibgeschützt.|
|isDefault|Boolescher Wert|Gibt an, ob dies Vereinbarung Standarddatei ist, wenn keiner der Kulturen die Client-Vorgabe übereinstimmt. Wenn keine der Dateien als Standard gekennzeichnet sind, wird der ersten als Standard behandelt. Schreibgeschützt.|
|language|String|Kultur der Vereinbarung Datei im Format languagecode2-Land/regioncode2. languagecode2 ist eine zwei-Code aus Kleinbuchstaben ISO 639-1 abgeleitet. Land/regioncode2 ISO 3166 abgeleitet ist und in der Regel besteht aus zwei Großbuchstaben oder ein Sprachtag BCP 47 (z. B. En-US). Schreibgeschützt.|

## <a name="relationships"></a>Beziehungen
Keine.


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFile"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "language": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
