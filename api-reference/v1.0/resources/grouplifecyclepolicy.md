---
title: groupLifecyclePolicy-Ressourcentyp
description: Steht für eine Lebenszyklusrichtlinie für eine Office 365-Gruppe. Eine Lebenszyklusrichtlinie für eine Gruppe ermöglicht Administratoren das Festlegen eines Ablaufzeitraums für Gruppen. Zum Beispiel nach 180 Tagen läuft eine Gruppe ab. Wenn eine Gruppe den Ablaufzeitpunkt erreicht, müssen Besitzer der Gruppe die Gruppe in einem vom Administrator definierten Zeitintervall verlängern. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind. Der neue Ablaufzeitraum für die Gruppe lautet dann beispielsweise 180 Tage ab Verlängerung. Wenn die Gruppe nicht verlängert wird, läuft sie ab und wird gelöscht. Die Gruppe kann innerhalb von 30 Tagen nach Löschung wiederhergestellt werden.
ms.openlocfilehash: 3d0ed05aa77a763d1cfdeb7c27cc37ee8e45a8c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017190"
---
# <a name="grouplifecyclepolicy-resource-type"></a>groupLifecyclePolicy-Ressourcentyp

Steht für eine Lebenszyklusrichtlinie für eine Office 365-Gruppe. Eine Lebenszyklusrichtlinie für eine Gruppe ermöglicht Administratoren das Festlegen eines Ablaufzeitraums für Gruppen. Zum Beispiel nach 180 Tagen läuft eine Gruppe ab. Wenn eine Gruppe den Ablaufzeitpunkt erreicht, müssen Besitzer der Gruppe die Gruppe in einem vom Administrator definierten Zeitintervall verlängern. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der Tage verlängert, die in der Richtlinie definiert sind. Der neue Ablaufzeitraum für die Gruppe lautet dann beispielsweise 180 Tage ab Verlängerung. Wenn die Gruppe nicht verlängert wird, läuft sie ab und wird gelöscht. Die Gruppe kann innerhalb von 30 Tagen nach Löschung wiederhergestellt werden.

## <a name="methods"></a>Methoden

| Methode | Rückgabetyp | Beschreibung |
|:---------------|:--------|:----------|
|[Get groupLifecyclePolicy](../api/grouplifecyclepolicy-get.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) |Dient zum Lesen der Eigenschaften und der Beziehungen eines groupLifecyclePolicy-Objekts.|
|[List groupLifecyclePolicies](../api/grouplifecyclepolicy-list.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md)-Sammlung | Listet alle groupLifecyclePolicies auf. |
|[Update groupLifecyclePolicy](../api/grouplifecyclepolicy-update.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) | Aktualisiert ein groupLifecyclePolicy-Objekt. |
|[Delete groupLifecyclePolicy](../api/grouplifecyclepolicy-delete.md) | Keine | Löscht ein groupLifecyclePolicy-Objekt. |
|[Add a group to a groupLifecyclePolicy](../api/grouplifecyclepolicy-addgroup.md)|Keine| Fügt eine Gruppe zu einer Lebenszyklusrichtlinie hinzu. |
|[Remove a group from a groupLifecyclePolicy](../api/grouplifecyclepolicy-removegroup.md)|Keine| Entfernt eine Gruppe aus einer Lebenszyklusrichtlinie. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:---------------|:--------|:----------|
|alternateNotificationEmails|Zeichenfolge| Liste der E-Mail-Adressen, an die Benachrichtigungen für Gruppen ohne Besitzer gesendet werden sollen. Mehrere E-Mail-Adressen können durch ein Semikolon voneinander getrennt definiert werden. |
|groupLifetimeInDays|Int32| Anzahl von Tagen, bis eine Gruppe abläuft und verlängert werden muss. Sobald die Gruppe verlängert wurde, wird der Ablaufzeitraum für die Gruppe um die Anzahl der definierten Tage verlängert. |
|id|Guid| Ein eindeutiger Bezeichner für eine Richtlinie. Schreibgeschützt.|
|managedGroupTypes|Zeichenfolge| Der Gruppentyp, für den die Ablaufrichtlinie gilt. Mögliche Werte sind **Alle**, **Ausgewählte** oder **Keine**. |

## <a name="relationships"></a>Beziehungen

Keine.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->