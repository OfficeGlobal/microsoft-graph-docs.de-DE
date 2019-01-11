---
title: Ressourcentyp businessFlowTemplate
description: In Azure AD Access Feature, überprüft die `businesFlowTemplate` stellt eine Azure AD Business Flow-Vorlage. Der Bezeichner der Vorlage, beispielsweise zum Überprüfen der Gast Mitglieder einer Gruppe ist vom Anrufer bereitgestellt wird, wenn eine Überprüfung Access erstellen.
localization_priority: Normal
ms.openlocfilehash: cad361d6c2d2aba70b2623ddf272e1eba42fd93b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889026"
---
# <a name="businessflowtemplate-resource-type"></a>Ressourcentyp businessFlowTemplate

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

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

## <a name="see-also"></a>Weitere Artikel

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

<!-- {
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
