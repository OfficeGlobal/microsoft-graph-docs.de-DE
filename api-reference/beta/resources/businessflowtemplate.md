---
title: Ressourcentyp businessFlowTemplate
description: In Azure AD Access Feature, überprüft die `businesFlowTemplate` stellt eine Azure AD Business Flow-Vorlage. Der Bezeichner der Vorlage, beispielsweise zum Überprüfen der Gast Mitglieder einer Gruppe ist vom Anrufer bereitgestellt wird, wenn eine Überprüfung Access erstellen.
localization_priority: Normal
ms.openlocfilehash: 567a7f499e2fb493f3ca519e312e69fb43fe3b79
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529579"
---
# <a name="businessflowtemplate-resource-type"></a>Ressourcentyp businessFlowTemplate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

In der Azure AD [Access überprüft](accessreviews-root.md) -Funktion die `businesFlowTemplate` stellt eine Azure AD Business Flow-Vorlage. Der Bezeichner der Vorlage, beispielsweise zum Überprüfen der Gast Mitglieder einer Gruppe ist vom Anrufer bereitgestellt wird, wenn eine Überprüfung Access erstellen.

Der Fluss Vorlage Geschäftsobjekte sind automatisch generiert, wenn die Onboards globaler Administrator den Mandanten so verwenden Sie das Access Feature überprüft.  Keine zusätzliche Business Fluss Vorlagen können erstellt werden.


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste businessFlowTemplates](../api/businessflowtemplate-list.md) | [BusinessFlowTemplate](businessflowtemplate.md) -Auflistung| Rufen Sie die Vorlagen für Unternehmen Fluss Bewertungen Zugriff auf entsprechende.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| `id`                     |`String`                | Das Feature zugewiesene Bezeichner der Vorlage Fluss business                                      |
| `displayName`            |`String`                | Der Name der Vorlage Fluss business                                                             |


## <a name="relationships"></a>Beziehungen

Keine.

## <a name="see-also"></a>Siehe auch

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Erstellen von accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Erstellen Sie eine neue AccessReview. |


## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.businessFlowTemplate"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/businessflowtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
