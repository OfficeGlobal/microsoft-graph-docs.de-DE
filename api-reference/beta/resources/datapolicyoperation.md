---
title: Ressourcentyp dataPolicyOperation
description: Stellt einen gesendete Daten Richtlinie Vorgang dar. Sie enthält die erforderlichen Informationen für das Nachverfolgen des Status eines Vorgangs. Beispielsweise kann ein Unternehmensadministrator anfordern, Daten Richtlinie Vorgang zum Exportieren eines Mitarbeiters Unternehmensdaten verwendet, und klicken Sie dann die Anforderung später verfolgen.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d3ec392bb30614346d2726262851eebc29ee779
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938748"
---
# <a name="datapolicyoperation-resource-type"></a>Ressourcentyp dataPolicyOperation

Stellt einen gesendete Daten Richtlinie Vorgang dar. Sie enthält die erforderlichen Informationen für das Nachverfolgen des Status eines Vorgangs. Beispielsweise kann ein Unternehmensadministrator anfordern, Daten Richtlinie Vorgang zum Exportieren eines Mitarbeiters Unternehmensdaten verwendet, und klicken Sie dann die Anforderung später verfolgen.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von dataPolicyOperation](../api/datapolicyoperation-get.md) | [dataPolicyOperation](datapolicyoperation.md) |Lesen Sie die Eigenschaften des DataPolicyOperation-Objekts.|

## <a name="properties"></a>Eigenschaften

> **Hinweis:** Alle Eigenschaften dieser Ressource sind schreibgeschützt.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|completedDateTime|DateTimeOffset|Stellt die bei die Anforderung für diese Richtlinie Datenvorgangs, in UTC-Zeit mit abgeschlossen wurde im ISO 8601-Format. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. "NULL", bis der Vorgang abgeschlossen ist.|
|id|Zeichenfolge| Eindeutiger Schlüssel für diesen Vorgang. |
|status|string| Mögliche Werte sind: `notStarted`, `running`, `complete`, `failed` und `unknownFutureValue`.|
|storageLocation|Zeichenfolge|Der URL-Adresse an, in dem Daten für exportanforderungen exportiert werden.|
|userId|Zeichenfolge|Die Id für den Benutzer, auf dem die Operation ausgeführt wird.|
|submittedDateTime|DateTimeOffset|Stellt die bei die Anforderung für diesen Datenvorgang im ISO 8601-Format verwenden übermittelt wurde, im UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|progress|Gleitkommawert mit doppelter Genauigkeit|Gibt den Fortschritt eines Vorgangs an.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)",
  "progress": "Double"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
