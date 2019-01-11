---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
ms.openlocfilehash: 78e4d1aff2003cc6d23580f4e52b46667cf6a9e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841706"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="01cb1-102">EditAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="01cb1-102">EditAction resource type</span></span>

> <span data-ttu-id="01cb1-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="01cb1-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01cb1-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="01cb1-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01cb1-105">Wenn eine **EditAction**-Ressource für eine [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität ein Element bearbeitet hat.</span><span class="sxs-lookup"><span data-stu-id="01cb1-105">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="01cb1-106">**Hinweis**: Diese Ressource ist heute zwar leer, in künftigen API-Überarbeitungen wird die Ressource aber möglicherweise mit weiteren Eigenschaften gefüllt.</span><span class="sxs-lookup"><span data-stu-id="01cb1-106">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="01cb1-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="01cb1-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="01cb1-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="01cb1-108">Properties</span></span>

<span data-ttu-id="01cb1-109">Keine.</span><span class="sxs-lookup"><span data-stu-id="01cb1-109">None.</span></span> <span data-ttu-id="01cb1-110">Dieses Facet ist ein NULL- oder Nicht-NULL-Wert und enthält keine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="01cb1-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="01cb1-111">Hinweise</span><span class="sxs-lookup"><span data-stu-id="01cb1-111">Remarks</span></span>

<span data-ttu-id="01cb1-112">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="01cb1-112">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction"
} -->
