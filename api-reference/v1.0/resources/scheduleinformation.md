---
title: scheduleInformation-Ressourcentyp
description: Stellt die Verfügbarkeit eines Benutzers, einer Verteilerliste oder einer Ressource für einen bestimmten Zeitraum dar.
localization_priority: Normal
ms.openlocfilehash: a19689eeafe9723cdadeb6147700933ab171637c
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30926607"
---
# <a name="scheduleinformation-resource-type"></a>scheduleInformation-Ressourcentyp

Stellt die Verfügbarkeit eines Benutzers, einer Verteilerliste oder einer Ressource (Raum oder Equipment) für einen bestimmten Zeitraum dar.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|availabilityView |Zeichenfolge |Stellt eine zusammengeführte Ansicht der Verfügbarkeit aller Elemente in `scheduleItems`dar. Die Ansicht besteht aus Zeitschlitzen. Die Verfügbarkeit in jedem Zeitschlitz wird mit `0`: = Free `1`, = zaghaft `2`, = busy `3`, = Abwesenheit, `4`= arbeiten an einem anderen Ort angezeigt.|
|error |[freeBusyError](freebusyerror.md) |Fehlerinformationen aus dem Versuch, die Verfügbarkeit des Benutzers, der Verteilerliste oder der Ressource abzurufen. |
|scheduleId |Zeichenfolge |Eine SMTP-Adresse des Benutzers, der Verteilerliste oder der Ressource, die eine Instanz von **scheduleInformation**identifiziert. |
|scheduleItems |[scheduleItem](scheduleitem.md) -Sammlung |Enthält die Elemente, die die Verfügbarkeit des Benutzers oder der Ressource beschreiben. |
|workingHours |[workingHours](workinghours.md) |Die Wochentage und Zeiten in einer bestimmten Zeitzone, an bzw. zu denen der Benutzer arbeitet. Diese werden als Teil des [Mailbox Settings](mailboxsettings.md)des Benutzers festgelegt.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
