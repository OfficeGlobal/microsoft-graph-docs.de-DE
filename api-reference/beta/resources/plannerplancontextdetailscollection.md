---
title: Ressourcentyp plannerPlanContextDetailsCollection
description: " der Wert ist das PlannerPlanContextDetails-Objekt."
author: TarkanSevilmis
ms.openlocfilehash: 725239a83f1c059aeef39f68b0d4d58ce8c91013
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346767"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a>Ressourcentyp plannerPlanContextDetailsCollection

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.


Die Ressource **PlannerPlanContextDetailsCollection** stellt die Auflistung von externen Kontexten mit denen ein Plans verknüpft ist. Diese Ressource ist ein offener Typ und ist Teil des [PlannerPlanDetails](plannerplandetails.md) -Objekts. Der Name der Eigenschaft in der Eigenschaft-Wert-Paar ist ein app-spezifischen Bezeichner des Kontexts. der Wert ist das [PlannerPlanContextDetails](plannerplancontextdetails.md) -Objekt.


## <a name="properties"></a>Eigenschaften
Eigenschaften vom Typ open können vom Client definiert werden. In diesem Fall sollte der Client einen charakteristischen Bezeichner verwenden, der den externen Kontext wie der Name der Eigenschaft darstellt. Die Eigenschaftswerte muss [PlannerPlanContextDetails](plannerplancontextdetails.md) -Objekte. Basierend auf OData, Eigenschaftennamen im offenen Typen die folgenden Zeichen nicht enthalten: `.`, `:`, `@`, `%`. Diese Zeichen mit URL-Codierung Format codiert werden müssen. Um ein Element in der Liste der Favoriten zu entfernen, muss der Wert aus der Auflistung [PlannerPlanContextCollection](plannerplancontextcollection.md) stattdessen entfernt werden die wird automatisch den Eintrag in diesem Objekt zu entfernen.


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
