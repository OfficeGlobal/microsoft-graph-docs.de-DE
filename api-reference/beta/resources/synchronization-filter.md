---
title: Filtertyp-Ressource
description: Bestimmt, welche Objekte für die Anwendung bereitgestellt werden soll. Angenommen, möchten Sie nur für Benutzer bereitgestellt werden soll, die sich in den USA befinden. Wenn ein Filter Gültigkeitsbereichs vorhanden ist, werden Objekte, die nicht den Filter erfüllen während der Synchronisierung übersprungen.
ms.openlocfilehash: 72885cfbd49083ce80b96cd389286d5c50937ffb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061508"
---
# <a name="filter-resource-type"></a>Filtertyp-Ressource

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Bestimmt, welche Objekte für die Anwendung bereitgestellt werden soll. Angenommen, möchten Sie nur für Benutzer bereitgestellt werden soll, die sich in den USA befinden. Wenn ein Filter Gültigkeitsbereichs vorhanden ist, werden Objekte, die nicht den Filter erfüllen während der Synchronisierung übersprungen.

Filter ist Teil der [Objekt-Zuordnung](synchronization-objectmapping.md). Es besteht aus mehreren Gruppen Filter aus, und jeder Filtergruppe enthält eine oder mehrere Klauseln. Ein Objekt gilt für die Gruppe im Bereich (die Gruppe ausgewertet wird, um `true`) nur dann, wenn alle Klauseln der Gruppe für ausgewertet werden `true`.

Ein Objekt gilt im Bereich für die Gruppe ein (Gruppe ausgewertet wird, um `true`), wenn die Gruppen in der Gruppe wird ausgewertet `true`.

Weitere Informationen finden Sie unter [attributbasierte Anwendung provisioning mit Gültigkeitsbereichs Filter](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|categoryFilterGroups|[FilterGroup](synchronization-filtergroup.md) -Auflistung|`*Experimental*`Filter für Gruppe festgelegt werden, ob die angegebene Objekt gehört und im Rahmen dieser Zuordnung Objekt verarbeitet werden soll. Ein Objekt gilt im Bereich *, wenn die Gruppen in der Auflistung ausgewertet wird, um `true` *.|
|Gruppen|[FilterGroup](synchronization-filtergroup.md) -Auflistung|Filter verwendet, um zu entscheiden, ob das angegebene Objekt in den Bereich für die Bereitstellung ist Gruppe festgelegt. **Dies ist der Filter, die in den meisten Fällen verwendet werden soll**. Wenn ein Objekt verwendet, um diesen Filter zu einem bestimmten Zeitpunkt, zu erfüllen und klicken Sie dann auf das Objekt oder die Filter geändert wurde, sodass dieser Filter nicht ist mehr, entsprechendes Objekt erfüllt * erhalten Ihre Bereitstellung ". Ein Objekt gilt im Bereich *, wenn die Gruppen in der Auflistung ausgewertet wird, um `true` *.|
|inputFilterGroups|[FilterGroup](synchronization-filtergroup.md) -Auflistung|`*Experimental*`Filter zum Herausfiltern von Objekten im frühen Stadium aus dem Verzeichnis zu lesen Gruppe festgelegt. Wenn ein Objekt nicht diesen Filter entsprechen wird es nicht weiter verarbeitet werden. Wichtig zu verstehen, wenn ein Objekt verwendet, um diesen Filter zu einem bestimmten Zeitpunkt zu erfüllen, und klicken Sie dann das Objekt oder die Filter geändert wurde, ist dieser Filter nicht mehr erfüllt ist, das Objekt Netzwerktools *nicht Ihre Bereitstellung abgerufen wird*. Ein Objekt gilt im Bereich *, wenn die Gruppen in der Auflistung ausgewertet wird, um `true` *. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filter"
}-->

```json
{
  "categoryFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "groups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "inputFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->