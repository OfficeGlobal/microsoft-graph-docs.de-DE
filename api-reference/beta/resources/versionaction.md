---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
ms.openlocfilehash: 1f315b26c45e337986784200fb6ec2c78612344b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866710"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="16c24-102">VersionAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="16c24-102">VersionAction resource type</span></span>

> <span data-ttu-id="16c24-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="16c24-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16c24-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16c24-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16c24-105">Wenn die **VersionAction**-Ressource für eine [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität eine neue Version erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="16c24-105">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="16c24-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="16c24-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

## <a name="properties"></a><span data-ttu-id="16c24-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16c24-107">Properties</span></span>

| <span data-ttu-id="16c24-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="16c24-108">Property name</span></span> | <span data-ttu-id="16c24-109">Typ</span><span class="sxs-lookup"><span data-stu-id="16c24-109">Type</span></span>   | <span data-ttu-id="16c24-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16c24-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="16c24-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="16c24-111">newVersion</span></span>    | <span data-ttu-id="16c24-112">string</span><span class="sxs-lookup"><span data-stu-id="16c24-112">string</span></span> | <span data-ttu-id="16c24-113">Der Name der neuen Version, die von dieser Aktion erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="16c24-113">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="16c24-114">Hinweise</span><span class="sxs-lookup"><span data-stu-id="16c24-114">Remarks</span></span>

<span data-ttu-id="16c24-115">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="16c24-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction"
} -->
