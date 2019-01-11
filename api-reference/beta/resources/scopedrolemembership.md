---
title: Ressourcentyp scopedRoleMembership
description: Ein Bereich Rollenmitgliedschaften beschreibt eines Benutzers Mitgliedschaft einer Directory-Rolle, die weiter an eine Administrative Einheit (AU) begrenzt ist.  Dies bietet einen Mechanismus, um einen Mandanten gesamte Unternehmen Adminsistrator zum Delegieren der administrativer Berechtigungen zu einem Benutzer das Verwalten von Benutzern und Gruppen in einer Teilmenge der Organisation (der Teilmenge von einer AU definiert wird) zu ermöglichen.
localization_priority: Normal
ms.openlocfilehash: a83acf82eadd9798a86a1a6456d5b2c4ca60be73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884798"
---
# <a name="scopedrolemembership-resource-type"></a>Ressourcentyp scopedRoleMembership

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Ein Bereich Rollenmitgliedschaften beschreibt eines Benutzers Mitgliedschaft einer Directory-Rolle, die weiter an eine Administrative Einheit (AU) begrenzt ist.  Dies bietet einen Mechanismus, um einen Mandanten gesamte Unternehmen Adminsistrator zum Delegieren der administrativer Berechtigungen zu einem Benutzer das Verwalten von Benutzern und Gruppen in einer Teilmenge der Organisation (der Teilmenge von einer AU definiert wird) zu ermöglichen.

## <a name="methods"></a>Methoden
Direkte Abfragen an diese Ressource werden nicht unterstützt.  Finden Sie im Thema [Administrative Einheiten](administrativeunit.md) zu Informationen zum Abfrage für bezogenen Rollenmitgliedschaften sowie hinzufügen und Entfernen von bezogenen-Rollenmitgliedschaften finden Sie unter. 

## <a name="properties"></a>Eigenschaften
| Eigenschaft   | Typ | Beschreibung |
|:---------------|:--------|:----------|
|administrativeUnitId|string|Eindeutiger Bezeichner für die administrative Einheit, der die Directory-Rolle zugeordnet ist|
|id|string| Eindeutiger Bezeichner für den Gültigkeitsbereich Rollenmitgliedschaften. Schreibgeschützt.|
|roleId|string| Eindeutiger Bezeichner für die Directory-Rolle, der in der Member ist.|
|roleMemberInfo|[identity](identity.md)| Rolle Mitglied Identitätsinformationen. Stellt den Benutzer, der Mitglied dieser bezogenen-Rolle ist.|

## <a name="relationships"></a>Beziehungen
Keine


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedrolemembership"
}-->

```json
{
  "administrativeUnitId": "string",
  "id": "string (identifier)",
  "roleId": "string",
  "roleMemberInfo": {"@odata.type": "microsoft.graph.identity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
