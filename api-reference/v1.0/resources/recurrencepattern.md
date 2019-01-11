---
title: recurrencePattern-Ressourcentyp
description: 'Beschreibt die Häufigkeit, mit der sich ein wiederkehrendes Ereignis wiederholt. '
localization_priority: Normal
ms.openlocfilehash: ebdb8a71d9f3acfb40191a7148f55999f6158aa1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892183"
---
# <a name="recurrencepattern-resource-type"></a>recurrencePattern-Ressourcentyp

Beschreibt die Häufigkeit, mit der sich ein wiederkehrendes [Ereignis](event.md) wiederholt. 

Je nach Ihrem Szenario können das Serienmuster einer Ereignisserie auf die sechs folgenden Arten angeben. Geben Sie für jeden Mustertyp die Zeitdauer zwischen Vorkommen an. Die tatsächlichen Vorkommen des wiederkehrenden Ereignisses folgen immer diesem Muster, das in den Datumsbereich fällt, den Sie für das Ereignis angeben. Ein wiederkehrendes Ereignis wird immer durch sein **recurrencePattern** (wie oft sich das Ereignis wiederholt), und seinen [recurrenceRange](recurrencerange.md) (über welchen Zeitraum sich das Ereignis wiederholt) definiert.

Verwenden Sie die **type**-Eigenschaft, um die unterschiedlichen Typen von **recurrencePattern** anzugeben, und die **interval**-Eigenschaft, um die Zeit zwischen Vorkommen anzugeben, die je nach **type** eine Anzahl von Tagen, Wochen, Monaten oder Jahren sein kann. Beachten Sie, welche Eigenschaften für jeden Typ erforderlich sind, wie in der folgenden Tabelle beschrieben.

> **Hinweis** Schließen Sie nur die Eigenschaften ein, die Sie für ein Serienmuster benötigen. Jede Eigenschaft, die Sie einschließen, die keinen unterstützten Typ aufweist, würde einen Fehler zurückgeben.

| Typ des Serienmusters | Wert der type-Eigenschaft | Beschreibung | Beispiel | Erforderliche Eigenschaften |
|:---------------|:--------|:--------|:--------|:----------|
| Täglich | `daily` | Das Ereignis wiederholt sich basierend auf der Anzahl von Tagen, die von **interval** zwischen den einzelnen Vorkommen angegeben werden. | Ereignis alle 3 Tage wiederholen | **type**, **interval** |
| Wöchentlich | `weekly` | Das Ereignis wird am gleichen Tag oder an den gleichen Tagen einer Woche basierend auf der Anzahl von Wochen zwischen zwei Vorkommen wiederholt. | Ereignis jeden Montag und Dienstag wiederholen | **type**, **interval**, **daysOfWeek**, **firstDayOfWeek** |
| Absolut monatlich | `absoluteMonthly` | Das Ereignis wird an dem angegebenen Tag des Monats (z. B. am 15.) basierend auf der Anzahl von Monaten zwischen den Vorkommen wiederholt. | Ereignis vierteljährlich (alle 3 Monate) am 15. wiederholen | **type**, **interval**, **dayOfMonth** |
| Relativ monatlich | `relativeMonthly` | Das Ereignis wird an dem angegebenen Tag oder an den angegebenen Tagen der Woche in derselben relativen Position im Monat basierend auf der Anzahl von Monaten zwischen den Vorkommen wiederholt. | Ereignis am zweiten Donnerstag oder Freitag alle drei Monate wiederholen | **type**, **interval**, **daysOfWeek** |
| Absolut jährlich | `absoluteYearly` | Das Ereignis wird an dem angegebenen Tag und Monat basierend auf der Anzahl von Jahren zwischen den Vorkommen wiederholt. | Ereignis am 15. März alle 3 Jahre wiederholen | **type**, **interval**, **dayOfMonth**, **month** |
| Relativ jährlich | `relativeYearly` | Das Ereignis wird an dem angegebenen Tag oder an den angegebenen Tagen der Woche in derselben relativen Position in einem bestimmten Monat des Jahres basierend auf der Anzahl von Jahren zwischen den Vorkommen wiederholt. | Ereignis am zweiten Donnerstag oder Freitag jeden November alle 3 Jahre wiederholen | **type**, **interval**, **daysOfWeek**, **month** |


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|dayOfMonth|Int32|Der Tag des Monats, an dem das Ereignis stattfindet. Erforderlich, wenn **type** `absoluteMonthly` oder `absoluteYearly` ist. |
|daysOfWeek|DayOfWeek-Auflistung|Eine Auflistung der Tage der Woche, an denen das Ereignis stattfindet. Die möglichen Werte sind: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`. <br>Wenn **type** `relativeMonthly` oder `relativeYearly` ist und **daysOfWeek** mehr als einen Tag angibt, fällt das Ereignis auf den ersten Tag, der dem Muster entspricht. <br> Erforderlich, wenn **type** `weekly`, `relativeMonthly` oder `relativeYearly` ist.|
|firstDayOfWeek|dayOfWeek|Der erste Tag der Woche. Die möglichen Werte sind: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`. Der Standardwert lautet `sunday`. Erforderlich, wenn **type** `weekly` ist. |
|Index|weekIndex|Gibt an, in welcher Instanz der zulässigen Tage, die unter **daysOfsWeek** angegeben sind, das Ereignis eintritt, ausgehend von der ersten Instanz des Monats gezählt. Die möglichen Werte sind: `first`, `second`, `third`, `fourth`, `last`. Der Standardwert lautet `first`. Optional; wird verwendet, wenn **type** `relativeMonthly` oder `relativeYearly` ist. |
|Intervall|Int32|Die Anzahl von Einheiten zwischen den Vorkommen, wobei Einheiten je nach **type** in Tagen, Wochen, Monaten oder Jahren angegeben werden können. Erforderlich. |
|Monat|Int32|Der Monat, in dem das Ereignis stattfindet.  Dies ist eine Zahl zwischen 1 und 12.|
|Typ|recurrencePatternType|Typ des Serienmusters: `daily`, `weekly`, `absoluteMonthly`, `relativeMonthly`, `absoluteYearly`, `relativeYearly`. Erforderlich.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recurrencePattern"
}-->

```json
{
  "dayOfMonth": 1024,
  "daysOfWeek": ["String"],
  "firstDayOfWeek": "String",
  "index": "String",
  "interval": 1024,
  "month": 1024,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recurrencePattern resource",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/recurrencepattern.md/microsoft.graph.recurrencePattern/daysOfWeek:
      Inconsistent types between parameter (String) and table (Object)"
  ],
  "tocPath": ""
}-->
