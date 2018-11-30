---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
ms.openlocfilehash: 041552f88561981338fa2ea5719d5af102fb3574
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060649"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="8bb1e-102">DeleteAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8bb1e-102">DeleteAction resource type</span></span>

> <span data-ttu-id="8bb1e-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8bb1e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bb1e-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8bb1e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8bb1e-105">Wenn eine **DeleteAction**-Ressource für eine [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität ein Element gelöscht hat.</span><span class="sxs-lookup"><span data-stu-id="8bb1e-105">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8bb1e-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8bb1e-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

## <a name="properties"></a><span data-ttu-id="8bb1e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8bb1e-107">Properties</span></span>

| <span data-ttu-id="8bb1e-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="8bb1e-108">Property name</span></span> | <span data-ttu-id="8bb1e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8bb1e-109">Type</span></span>   | <span data-ttu-id="8bb1e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8bb1e-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8bb1e-111">name</span><span class="sxs-lookup"><span data-stu-id="8bb1e-111">name</span></span>          | <span data-ttu-id="8bb1e-112">string</span><span class="sxs-lookup"><span data-stu-id="8bb1e-112">string</span></span> | <span data-ttu-id="8bb1e-113">Der Name des Elements, das gelöscht wurde.</span><span class="sxs-lookup"><span data-stu-id="8bb1e-113">The name of the item that was deleted.</span></span>
| <span data-ttu-id="8bb1e-114">objectType</span><span class="sxs-lookup"><span data-stu-id="8bb1e-114">objectType</span></span>    | <span data-ttu-id="8bb1e-115">string</span><span class="sxs-lookup"><span data-stu-id="8bb1e-115">string</span></span> | <span data-ttu-id="8bb1e-116">`File`oder `Folder`, je nach Typ des gelöschten Elements.</span><span class="sxs-lookup"><span data-stu-id="8bb1e-116">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="8bb1e-117">Hinweise</span><span class="sxs-lookup"><span data-stu-id="8bb1e-117">Remarks</span></span>

<span data-ttu-id="8bb1e-118">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="8bb1e-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction"
} -->
