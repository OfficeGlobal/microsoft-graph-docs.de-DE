---
title: exclusionGroupAssignmentTarget-Ressourcentyp
description: Steht für eine Gruppe, die aus einer Zuweisung ausgeschlossen werden sollte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 24e732bc0c48c9c25f35da1afbccef04d17fe0cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919862"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="6fa9d-103">exclusionGroupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6fa9d-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="6fa9d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6fa9d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fa9d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6fa9d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fa9d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6fa9d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fa9d-107">Steht für eine Gruppe, die aus einer Zuweisung ausgeschlossen werden sollte.</span><span class="sxs-lookup"><span data-stu-id="6fa9d-107">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="6fa9d-108">Erbt von [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6fa9d-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6fa9d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6fa9d-109">Properties</span></span>
|<span data-ttu-id="6fa9d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6fa9d-110">Property</span></span>|<span data-ttu-id="6fa9d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6fa9d-111">Type</span></span>|<span data-ttu-id="6fa9d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6fa9d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fa9d-113">groupId</span><span class="sxs-lookup"><span data-stu-id="6fa9d-113">groupId</span></span>|<span data-ttu-id="6fa9d-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6fa9d-114">String</span></span>|<span data-ttu-id="6fa9d-115">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="6fa9d-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="6fa9d-116">Vererbt von [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6fa9d-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fa9d-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6fa9d-117">Relationships</span></span>
<span data-ttu-id="6fa9d-118">Keine</span><span class="sxs-lookup"><span data-stu-id="6fa9d-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6fa9d-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6fa9d-119">JSON Representation</span></span>
<span data-ttu-id="6fa9d-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6fa9d-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```





