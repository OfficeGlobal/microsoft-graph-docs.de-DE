---
title: Ressourcentyp TeamsTabConfiguration (Open Type)
description: Die Einstellungen, die den Inhalt einer Registerkarte bestimmen.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 515e5896591b58054f161ff740f68b0ca4913663
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913485"
---
# <a name="teamstabconfiguration-resource-type-open-type"></a>Ressourcentyp TeamsTabConfiguration (Open Type)

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die Einstellungen, die den Inhalt einer [Registerkarte](teamstab.md)bestimmen. Wenn eine Registerkarte interaktiv konfiguriert ist, wird diese Informationen von der Registerkarte Anbieter-Anwendung festgelegt.
Abgesehen von den Eigenschaften geben Anwendungsbeispiele Anbieter Registerkarte zusätzliche benutzerdefinierte Eigenschaften.

## <a name="properties"></a>Eigenschaften

|Eigenschaft|Typ|Beschreibung|
|-|-|-|
|  entityId   |   string |  Der Bezeichner für die Entität, die von der Registerkarte Anbieter gehostet werden.     |
|  contentUrl |   string |  URL für das rendering von Inhalt in Teams Registerkarten verwendet. Erforderlich.    |
|  removeUrl  |   string |  URL von Teams Client aufgerufen, wenn eine Registerkarte mithilfe des Teams Clients entfernt wird.     |
|  websiteUrl |   string |  URL für die Anzeige der Registerkarte Inhalt außerhalb von Teams.     |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTabConfiguration"
}-->

```json
{
   "entityId": "string",
   "contentUrl": "string (HTTPS Url)",
   "websiteUrl": "string (HTTPS Url)",
   "removeUrl": "string (HTTPS Url)"  
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsTabConfiguration complex type (Open Type)",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
