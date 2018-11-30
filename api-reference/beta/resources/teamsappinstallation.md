---
title: Ressourcentyp teamsAppInstallation
description: 'Eine TeamsApp in einem Team installiert. '
ms.openlocfilehash: 64573e163c0ec5ce9f3282e747dffd4ccc6718de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061145"
---
# <a name="teamsappinstallation-resource-type"></a>Ressourcentyp teamsAppInstallation

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Eine [TeamsApp](teamsapp.md) in einem [Team](team.md)installiert. Alle Bots, die Teil der app sind wird in jedem Team aufgenommen, die, denen die app hinzugefügt wird.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Liste apps](../api/teamsappinstallation-list.md) | [teamsAppInstallation](teamsapp.md) | Listet die apps in einem Team installiert.|
|[Hinzufügen der app](../api/teamsappinstallation-add.md) | [teamsAppInstallation](teamsapp.md) | Fügt (installiert) einer app zu einem Team.|
|[Entfernen der app](../api/teamsappinstallation-delete.md) | Keines | Entfernt (deinstalliert) einer app aus einem Team.|
|[Aktualisieren der app](../api/teamsappinstallation-delete.md) | Keines | Upgrades auf die neueste Version der app.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft            | Typ     | Beschreibung |
|:------------------- |:-------- |:----------- |
| id                  | string   | Eine eindeutige Id (nicht die Teams Appid). |

## <a name="relationships"></a>Beziehungen

| Beziehung   | Typ    | Beschreibung |
|:---------------|:--------|:----------|
|teamsApp|[teamsApp](teamsapp.md)| Die app, die installiert ist. |
|teamsAppDefinition|[teamsAppDefinition](teamsapp.md)| Die Details dieser Version der app. |

## <a name="json-representation"></a>JSON-Darstellung

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string",
}
```

# <a name="see-also"></a>Siehe auch

- [teamsApp](teamsapp.md)
- [teamsAppDefinition](teamsappdefinition.md)
- [teamsTab](../resources/teamstab.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teamsApp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

