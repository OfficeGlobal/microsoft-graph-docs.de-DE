---
title: messageRule-Ressourcentyp
description: Eine Regel, die auf Nachrichten im Posteingang eines Benutzers angewendet wird.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 9336f2e35d6c68d86c3e92b5f94c024eff1e49a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862125"
---
# <a name="messagerule-resource-type"></a>messageRule-Ressourcentyp


Eine Regel, die auf Nachrichten im Posteingang eines Benutzers angewendet wird.

In Outlook können Sie Regeln für eingehende Nachrichten im Posteingang festlegen, um bestimmte Aktionen bei bestimmten Bedingungen auszuführen. 

Programmgesteuert können Sie über die **messageRules**-Navigationseigenschaft des [Posteingangsordners](mailfolder.md) auf Regeln zugreifen. Jede Regel wird von dieser **messageRule**-Ressource dargestellt, verfügbare Regelaktionen werden von dem komplexen Typ [messageRuleActions](messageruleactions.md) dargestellt, und verfügbare Regelbedingungen und -ausnahmen werden von dem komplexen Typ [messageRulePredicates](messagerulepredicates.md) dargestellt.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| Aktionen | [messageRuleActions](messageruleactions.md) | Aktionen, die auf eine Nachricht angewendet werden, wenn die entsprechenden Bedingungen erfüllt sind. |
| Bedingungen | [messageRulePredicates](messagerulepredicates.md) | Bedingungen, die bei Erfüllung die entsprechenden Aktionen für diese Regel auslösen. |
| displayName | Zeichenfolge | Der Anzeigename der Regel. |
| Ausnahmen | [messageRulePredicates](messagerulepredicates.md) | Ausnahmebedingungen für die Regel. |
| hasError | Boolescher Wert | Gibt an, ob sich die Regel in einem Fehlerzustand befindet. Schreibgeschützt. |
| id |Zeichenfolge|Der eindeutige Bezeichner der Regel. Schreibgeschützt.|
| isEnabled | Boolescher Wert | Gibt an, ob die Regel auf Nachrichten angewendet werden kann. |
| isReadOnly | Boolescher Wert | Gibt an, ob die Regel schreibgeschützt ist und von der Regel-REST-API nicht geändert oder gelöscht werden kann. |
| sequence | Int32 | Gibt die Reihenfolge an, in der die Regel zusammen mit anderen Regeln ausgeführt wird. |


## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
   "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.messageRule"
}-->

```json
{
  "actions": {"@odata.type": "microsoft.graph.messageRuleActions"},
  "conditions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "displayName": "String",
  "exceptions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "hasError": "Boolean",
  "id": "String",
  "isEnabled": "Boolean",
  "isReadOnly": "Boolean",
  "sequence": "Int32"
}

```

## <a name="methods"></a>Methoden
| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Auflisten von Regeln](../api/mailfolder-list-messagerules.md) | [messageRule](messagerule.md)-Sammlung |Ruft alle **messageRule**-Objekte ab, die für das Postfach des Benutzers definiert sind.|
|[Regel abrufen](../api/messagerule-get.md) | [messageRule](messagerule.md) |Lesen der Eigenschaften und Beziehungen eines **messageRule**-Objekts.|
|[Erstellen](../api/mailfolder-post-messagerules.md) | [messageRule](messagerule.md) |Erstellen Sie ein  **messageRule**-Objekt, indem Sie eine Gruppe von Bedingungen und Aktionen angeben.|
|[Update](../api/messagerule-update.md) | [messageRule](messagerule.md) |Ändern Sie die schreibbaren Eigenschaften in einem **messageRule**-Objekt, und speichern Sie die Änderungen. |
|[Delete](../api/messagerule-delete.md) | Keine |Löschen des angegebenen **messageRule**-Objekts. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
