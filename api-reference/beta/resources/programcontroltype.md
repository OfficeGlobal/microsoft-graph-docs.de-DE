---
title: Ressourcentyp programControlType
description: 'In Azure AD Access Feature überprüft, der Steuerelementtyp Programm wird verwendet, wenn Zuordnen eines Steuerelements an ein Programm, den Typ des Access-Überprüfung an das Steuerelement ist.  '
localization_priority: Normal
ms.openlocfilehash: 0091c23fd5d537e7c1fd62051778e56b510a3dab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808232"
---
# <a name="programcontroltype-resource-type"></a>Ressourcentyp programControlType

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

In der Azure AD [Access überprüft](accessreviews-root.md) -Funktion wird der Programm Steuerelementtyp verwendet, wenn zuordnen ein Steuerelements an ein Programm, um den Typ des Access-Überprüfung anzugeben, die für das Steuerelement ist.  

Die Programm-Steuerelement Typ-Objekte werden automatisch generiert, wenn die Onboards globaler Administrator den Mandanten so verwenden Sie das Access Feature überprüft.  Keine zusätzliche Programm Steuerungstypen können erstellt werden.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste programControlTypes](../api/programcontroltype-list.md) | [ProgramControlType](programcontroltype.md) -Auflistung| Programm Steuerelement Listentypen. |

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Das Feature zugewiesenen Bezeichner des Typs Programm                                      |
| `displayName`            |`String`                | Der Name des Typs Programm                                                             |


## <a name="relationships"></a>Beziehungen

Keine.


## <a name="see-also"></a>Siehe auch

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Erstellen von programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Fügen Sie ein Programm ein ProgramControl hinzu.|


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
