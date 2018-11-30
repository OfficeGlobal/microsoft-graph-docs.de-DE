---
title: Ressourcentyp programControlType
description: 'In Azure AD Access Feature überprüft, der Steuerelementtyp Programm wird verwendet, wenn Zuordnen eines Steuerelements an ein Programm, den Typ des Access-Überprüfung an das Steuerelement ist.  '
ms.openlocfilehash: 8fc406648d8f8c943920507a5734f47d2add1b4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062122"
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
