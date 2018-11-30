---
title: Ressourcentyp scheduleInformation
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
ms.openlocfilehash: 0b7bbd861a044b28cd22603fd0ccc27d20f46fba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061469"
---
# <a name="scheduleinformation-resource-type"></a>Ressourcentyp scheduleInformation

 > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.
 
Stellt die Verfügbarkeit von einem Benutzer, eine Verteilerliste oder eine Ressource für einen angegebenen Zeitraum dar.

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|availabilityView |String |Stellt eine Ansicht der Verfügbarkeit aller Elemente in zusammengeführte `scheduleItems`. Die Ansicht Zeitfenster besteht aus. Verfügbarkeit während jedes Zeitintervall wird mit angegeben: `0`= frei, `1`mit Vorbehalt = `2`= beschäftigt, `3`= abwesend, `4`= arbeiten an anderer Stelle.|
|error |[freeBusyError](freebusyerror.md) |Fehlerinformationen versucht, die die Verfügbarkeit des Benutzers, der Verteilerliste oder der Ressource zu erhalten. |
|scheduleId |String |Eine SMTP-Adresse des Benutzers, der Verteilerliste oder der Ressource, die eine Instanz des **ScheduleInformation**identifiziert. |
|scheduleItems |[von ScheduleItem](scheduleitem.md) -Auflistung |Enthält die Elemente, die die Verfügbarkeit des Benutzers oder der Ressource zu beschreiben. |
|workingHours |[workingHours](workinghours.md) |Die Wochentage und Zeiten in einer bestimmten Zeitzone, an bzw. zu denen der Benutzer arbeitet. Diese werden als Teil des Benutzers [MailboxSettings](mailboxsettings.md)festgelegt.|


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
<!-- {
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->