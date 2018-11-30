---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CreateAction
ms.openlocfilehash: 4b5d6a50c37c04b1c708e798820b8295d89ebf80
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059476"
---
# <a name="createaction-resource-type"></a><span data-ttu-id="34f6d-102">CreateAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="34f6d-102">CreateAction resource type</span></span>

> <span data-ttu-id="34f6d-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="34f6d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34f6d-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34f6d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34f6d-105">Wenn eine **CreateAction**-Ressource für eine [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität ein Element erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="34f6d-105">The presence of the **CreateAction** resource on an [**itemActivity**][activity] indicates that the activity created an item.</span></span>

<span data-ttu-id="34f6d-106">**Hinweis**: Diese Ressource ist heute zwar leer, in künftigen API-Überarbeitungen wird die Ressource aber möglicherweise mit weiteren Eigenschaften gefüllt.</span><span class="sxs-lookup"><span data-stu-id="34f6d-106">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="34f6d-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="34f6d-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="34f6d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="34f6d-108">Properties</span></span>

<span data-ttu-id="34f6d-109">Keine.</span><span class="sxs-lookup"><span data-stu-id="34f6d-109">None.</span></span> <span data-ttu-id="34f6d-110">Dieses Facet ist ein NULL- oder Nicht-NULL-Wert und enthält keine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="34f6d-110">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="34f6d-111">Hinweise</span><span class="sxs-lookup"><span data-stu-id="34f6d-111">Remarks</span></span>

<span data-ttu-id="34f6d-112">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="34f6d-112">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The CreateAction object provides information about the creation of an item.",
  "keywords": "activities,activity,action,create,creation",
  "section": "documentation",
  "tocPath": "Resources/CreateAction"
} -->
