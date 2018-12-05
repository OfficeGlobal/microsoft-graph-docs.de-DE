---
title: workingHours-Ressourcentyp
description: Stellt die Wochentage und Zeiten in einer bestimmten Zeitzone dar, an bzw. zu denen der Benutzer arbeitet.
ms.openlocfilehash: 915ec185931d3f7e77f010517a3ef0c3bff92204
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063572"
---
# <a name="workinghours-resource-type"></a>workingHours-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Wochentage und Zeiten in einer bestimmten Zeitzone dar, an bzw. zu denen der Benutzer arbeitet.

Zugriff auf die Arbeitszeiten eines Benutzers ist bei der Aktivitäts- oder Ressourcenplanung hilfreich. Sie können die Arbeitszeiten eines Benutzers als Teil der [Postfacheinstellungen](mailboxsettings.md) des Benutzers [abrufen](../api/user-get-mailboxsettings.md#request-3) und [festlegen](../api/user-update-mailboxsettings.md#request-2) . 

Sie können für die Arbeitszeiten auch eine andere Zeitzone als die für Ihren Outlook-Client festgelegte Zeitzone festlegen. Dies kann zum Beispiel hilfreich sein, wenn Sie in eine andere Zeitzone reisen. Sie können den Outlook-Client auf  
die Zielzeitzone festlegen, sodass die Outlook-Zeitwerte in der lokalen Zeit angezeigt werden, solange Sie sich in dieser Zeitzone befinden.
Wenn andere Personen Arbeitsbesprechungen mit Ihnen an Ihrem üblichen Arbeitsplatz anfordern, können sie sich an Ihre Arbeitszeiten in der jeweiligen Zeitzone halten.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| daysOfWeek | Zeichenfolgenauflistung | Die Wochentage, an denen der Benutzer arbeitet. |
| startTime | Edm.TimeOfDay | Die Tageszeit, zu der der Benutzer zu arbeiten beginnt. |
| endTime | Edm.TimeOfDay | Die Tageszeit, zu der der Benutzer zu arbeiten aufhört. |
| timeZone | [timeZoneBase](timezonebase.md) | Die Zeitzone, für die die Arbeitszeiten gelten. |


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workingHours"
}-->

```json
{
  "daysOfWeek": ["string"],
  "startTime": "TimeOfDay",
  "endTime": "TimeOfDay",
  "timeZone": {"@odata.type": "microsoft.graph.timeZoneBase"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workingHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->