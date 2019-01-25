---
title: Programm Ressourcentyp
description: 'In Azure AD Access Feature überprüft, ein Programm ist ein Container, Programm Steuerelemente halten. Ein Mandant kann eine oder mehrere Programme verfügen.  Jedes Steuerelement verknüpft eine Überprüfung Zugriff auf ein Programm, um zugehörige Access findet erleichtern überprüft.  '
localization_priority: Normal
ms.openlocfilehash: 2498279f27f5859eadcfa1d70662e3d8f3b5246c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515188"
---
# <a name="program-resource-type"></a>Programm Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "program resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/program.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
