---
title: plannerOrderHintsByAssignee-Ressourcentyp
description: Die **PlannerOrderHintsByAssignee** ist eine Ressource, die Sortierung Hinweise für "assignees" in einer Ressource PlannerTask an, dass die Reihenfolge des Vorgangs in der Ansicht zugewiesen an der Aufgabe-Karte enthält.
localization_priority: Normal
ms.openlocfilehash: cdc254eab43972d321e01e646880b3087f3af6f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863945"
---
# <a name="plannerorderhintsbyassignee-resource-type"></a><span data-ttu-id="94107-103">plannerOrderHintsByAssignee-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="94107-103">plannerOrderHintsByAssignee resource type</span></span>

> <span data-ttu-id="94107-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="94107-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94107-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="94107-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94107-p102">Die **plannerOrderHintsByAssignee**-Ressource enthält [Anordnungshinweise](planner-order-hint-format.md) für zugewiesene Personen in einer [plannerTask](plannertask.md)-Ressource, um die Anordnung der Aufgabe in der Ansicht „ZugewiesenAn“ des Task Board anzugeben. Es handelt sich um einen offenen Typ. Die Eigenschaften sind die IDs der Benutzer, die der Aufgabe zugewiesen sind, und die Werte sind Anordnungshinweise.</span><span class="sxs-lookup"><span data-stu-id="94107-p102">The **plannerOrderHintsByAssignee** is a resource that contains [ordering hints](planner-order-hint-format.md) for assignees in a [plannerTask](plannertask.md) resource, to indicate the order of the task in Assigned To view of the Task Board. This type is an open type. The properties are the ids of users assigned to the task, and the values are order hints.</span></span>

## <a name="properties"></a><span data-ttu-id="94107-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="94107-109">Properties</span></span>
<span data-ttu-id="94107-p103">Eigenschaften mit offenem Typ können vom Client definiert werden. In diesem Fall muss der Client IDs von Benutzern, die der Aufgabe zugewiesen sind, als Eigenschaftennamen und einen gültigen [Anordnungshinweis](planner-order-hint-format.md) als Wert angeben. Von diesem Typ können keine Eigenschaften entfernt werden. Der Dienst entfernt automatisch Werte, wenn die Zuweisungen in der enthaltenden [plannerTask](plannertask.md)-Ressource aktualisiert werden.</span><span class="sxs-lookup"><span data-stu-id="94107-p103">Properties of an Open Type can be defined by the client. In this case, the client must provide ids of users assigned to the task as property names, and a valid [order hint](planner-order-hint-format.md) as the value. Properties cannot be removed from this type. The service will automatically remove values as the assignments on the containing [plannerTask](plannertask.md) are updated.</span></span>

<span data-ttu-id="94107-114">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="94107-114">Example:</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
}-->

```json
{
  "ca2a1df2-e36b-4987-9f6b-0ea462f4eb47": "String",
  "4e98f8f1-bb03-4015-b8e0-19bb370949d8": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerOrderHintsByAssignee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
