---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
ms.openlocfilehash: f22761dd713b6d09d5e6fafb765d6d43bfc81bf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060073"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="e0433-102">VersionAction-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e0433-102">VersionAction resource type</span></span>

> <span data-ttu-id="e0433-103">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e0433-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0433-104">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e0433-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e0433-105">Wenn die **VersionAction**-Ressource für eine [ **ItemActivity**][activity] vorhanden ist, bedeutet dies, dass die Aktivität eine neue Version erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="e0433-105">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e0433-106">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e0433-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e0433-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e0433-107">Properties</span></span>

| <span data-ttu-id="e0433-108">Eigenschaftenname</span><span class="sxs-lookup"><span data-stu-id="e0433-108">Property name</span></span> | <span data-ttu-id="e0433-109">Typ</span><span class="sxs-lookup"><span data-stu-id="e0433-109">Type</span></span>   | <span data-ttu-id="e0433-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e0433-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e0433-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="e0433-111">newVersion</span></span>    | <span data-ttu-id="e0433-112">string</span><span class="sxs-lookup"><span data-stu-id="e0433-112">string</span></span> | <span data-ttu-id="e0433-113">Der Name der neuen Version, die von dieser Aktion erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="e0433-113">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="e0433-114">Hinweise</span><span class="sxs-lookup"><span data-stu-id="e0433-114">Remarks</span></span>

<span data-ttu-id="e0433-115">Elementaktivitätsdatensätze sind zurzeit nur für SharePoint und OneDrive for Business verfügbar.</span><span class="sxs-lookup"><span data-stu-id="e0433-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction"
} -->
