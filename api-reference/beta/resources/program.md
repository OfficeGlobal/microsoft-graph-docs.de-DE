---
title: Programm Ressourcentyp
description: 'In Azure AD Access Feature überprüft, ein Programm ist ein Container, Programm Steuerelemente halten. Ein Mandant kann eine oder mehrere Programme verfügen.  Jedes Steuerelement verknüpft eine Überprüfung Zugriff auf ein Programm, um zugehörige Access findet erleichtern überprüft.  '
ms.openlocfilehash: cb08d0edb7487be95e159ed5e2a2546a92e7bce7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065331"
---
# <a name="program-resource-type"></a>Programm Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

In der Azure AD [Access überprüft](accessreviews-root.md) -Funktion ist ein Programm einen Container, halten Programm Steuerelemente. Ein Mandant kann eine oder mehrere Programme verfügen.  Jedes Steuerelement verknüpft eine Überprüfung Zugriff auf ein Programm, um zugehörige Access findet erleichtern überprüft.  

Jeder Mandant, die auf-Azure AD an hat Zugriff Bewertungen hat ein Programm `Default program`.  Ein globaler Administrator kann zusätzliche Programme, beispielsweise zum Darstellen der Compliance-Initiativen erstellen. 


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Erstellen der Anwendung](../api/program-create.md) |   [Programm](program.md)   |   Erstellen Sie ein neues Programm.|
|[Programm löschen](../api/program-delete.md) |   Keine.   |   Löschen eines Programms.|
|[Programme auflisten](../api/program-list.md) |  [Programm](program.md) -Auflistung|   Rufen Sie eine Auflistung aller Programme.|
|[Liste ProgramControls eines Programms](../api/program-listcontrols.md) |      [ProgramControl](programcontrol.md) -Auflistung| Rufen Sie eine Auflistung der Steuerelemente eines Programms.|
|[Update-Programm](../api/program-update.md) |   [Programm](program.md)|  Aktualisieren eines Programms.|

## <a name="permissions"></a>Berechtigungen

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | ProgramControl.Read.All ProgramControl.ReadWrite.All |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Nicht unterstützt |


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| `id`                        |`String`                              |  Das Feature zugewiesenen Bezeichner des Programms.                    |
| `displayName`               |`String`                              |  Der Name des Programms.  Erforderliche auf erstellen.                  |
| `description`               |`String`                              |  Die Beschreibung des Programms.           |

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| `controls`                  |[programControl](programcontrol.md) | Steuerelemente, die das Programm zugeordnet. |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.program"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "description": "string"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->