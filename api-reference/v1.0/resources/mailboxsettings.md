---
title: mailboxSettings-Ressourcentyp
description: Einstellungen für das primäre Postfach des angemeldeten Benutzers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 53ded2d60161d833f70a3b747e0ec35953d5bd39
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937082"
---
# <a name="mailboxsettings-resource-type"></a>mailboxSettings-Ressourcentyp

Einstellungen für das primäre Postfach des angemeldeten Benutzers.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|archiveFolder|string|Ordner-ID eines Archivordners für den Benutzer.|
|automaticRepliesSetting|[automaticRepliesSetting](automaticrepliessetting.md)|Konfigurationseinstellungen zum automatischen Benachrichtigen des Absenders bei eingehenden E-Mails mit einer Nachricht vom angemeldeten Benutzer.|
|language|[localeInfo](localeinfo.md)|Die Gebietsschemainformationen des Benutzers, einschließlich der bevorzugten Sprache und Land/Region.|
|timeZone|string|Die Standardzeitzone für das Postfach des Benutzers.|
|workingHours|[workingHours](workinghours.md)|Die Wochentage und Zeiten in einer bestimmten Zeitzone, an bzw. zu denen der Benutzer arbeitet.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
