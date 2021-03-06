---
title: recurrenceRange-Ressourcentyp
description: 'Beschreibt den Datumsbereich, über den sich ein wiederkehrendes Ereignis wiederholt. '
localization_priority: Normal
ms.openlocfilehash: cee5a06d8f76264cd7c98924c532c8f864cab87d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518968"
---
# <a name="recurrencerange-resource-type"></a>recurrenceRange-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Beschreibt den Datumsbereich, über den sich ein wiederkehrendes [Ereignis](event.md) wiederholt. 

Je nach Ihrem Szenario können Sie den Datumsbereich einer Ereignisserie in einer der drei folgenden Arten angeben. Sie müssen zwar immer einen **startDate**-Wert für den Datumsbereich angeben, Sie können aber auch ein wiederkehrendes Ereignis angeben, das an einen angegebenen Datum endet, das nicht endet oder das nach 5 Vorkommen endet. Beachten Sie, dass die tatsächlichen Vorkommen innerhalb des Datumsbereichs immer dem Serienmuster folgen, das Sie für das wiederkehrende Ereignis angeben. Ein wiederkehrendes Ereignis wird immer durch sein [recurrencePattern](recurrencepattern.md) (wie oft sich das Ereignis wiederholt), und seinen **recurrenceRange** (über welchen Zeitraum sich das Ereignis wiederholt) definiert.


## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|endDate|Date|Das Datum zum Beenden des Anwendens des Musters. Je nach dem Serienmuster des Ereignisses ist das letzte Vorkommen der Besprechung möglicherweise nicht an diesem Datum. Erforderlich, wenn **type** `endDate` ist.|
|numberOfOccurrences|Int32|Die Anzahl von Wiederholungen für das Ereignis. Erforderlich; muss positiv sein, wenn **type** `numbered` ist.|
|recurrenceTimeZone|String |Zeitzone für die **startDate**- und **endDate**-Eigenschaften. Optional. Falls nicht angegeben, wird die Zeitzone des Ereignisses verwendet.|
|startDate|Datum|Das Datum zum Starten des Anwendens des Musters. Je nach dem Serienmuster des Ereignisses findet das erste Vorkommen der Besprechung möglicherweise an diesem Datum oder später statt. Muss der gleiche Wert wie die **start**-Eigenschaft des wiederkehrenden [Ereignisses](event.md) sein. Erforderlich.|
|type|Zeichenfolge|Der Serienbereich. Mögliche Werte: `endDate`, `noEnd`, `numbered`. Erforderlich.|

Verwenden Sie die **type**-Eigenschaft, um die unterschiedlichen Typen von **recurrenceRange** anzugeben. Beachten Sie die erforderlichen Eigenschaften für jeden Typ, wie in der folgenden Tabelle beschrieben.

| Eigenschaft "type"  | Typ des Serienbereichs | Beschreibung | Beispiel | Erforderliche Eigenschaften |
|:-------|:---------------|:--------|:--------|:--------|
|`endDate` |Bereich mit Enddatum | Ereignis an allen Tagen wiederholen, die mit dem entsprechenden Serienmuster zwischen dem **startDate** und dem **endDate** übereinstimmen. | Ereignis im Datumsbereich zwischen 1. Juni 2017 und 15. Juni 2017 wiederholen. | **type**, **startDate**, **endDate** | 
|`noEnd`   |Bereich ohne Enddatum | Ereignis an allen Tagen wiederholen, die mit dem entsprechenden Serienmuster beginnend am **startDate** übereinstimmen. | Ereignis im Datumsbereich beginnend am 1. Juni 2017 unbegrenzt wiederholen. | **type**, **startDate** |
|`numbered`|Bereich mit einer bestimmten Anzahl von Vorkommen | Ereignis für die **numberOfOccurrences** basierend auf dem Serienmuster beginnend am **startDate** wiederholen. | Ereignis im Datumsbereich beginnend am 1. Juni 2017 für 10 Vorkommen wiederholen.  | **type**, **startDate**, **numberOfOccurrences** |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrenceRange"
}-->

```json
{
  "endDate": "String (timestamp)",
  "numberOfOccurrences": 1024,
  "recurrenceTimeZone": "string",
  "startDate": "String (timestamp)",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recurrenceRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Warning: /api-reference/beta/resources/recurrencerange.md:\r\n      Failed to parse any rows out of table with headers: | type property  | Type of recurrence range | Description | Example | Required properties |",
    "Error: /api-reference/beta/resources/recurrencerange.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
