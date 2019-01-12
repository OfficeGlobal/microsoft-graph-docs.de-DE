---
title: groupAssignmentTarget-Ressourcentyp
description: Stellt eine Zuweisung zu einer Gruppe dar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 96aec1b72233cfe7d553b8f17feb9af382d89cde
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971676"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="74757-103">groupAssignmentTarget-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="74757-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="74757-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="74757-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74757-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="74757-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74757-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="74757-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74757-107">Stellt eine Zuweisung zu einer Gruppe dar.</span><span class="sxs-lookup"><span data-stu-id="74757-107">Represents an assignment to a group.</span></span>

<span data-ttu-id="74757-108">Erbt von [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="74757-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="74757-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="74757-109">Properties</span></span>
|<span data-ttu-id="74757-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="74757-110">Property</span></span>|<span data-ttu-id="74757-111">Typ</span><span class="sxs-lookup"><span data-stu-id="74757-111">Type</span></span>|<span data-ttu-id="74757-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74757-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74757-113">groupId</span><span class="sxs-lookup"><span data-stu-id="74757-113">groupId</span></span>|<span data-ttu-id="74757-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="74757-114">String</span></span>|<span data-ttu-id="74757-115">Die Gruppen-ID, die das Ziel der Zuweisung ist.</span><span class="sxs-lookup"><span data-stu-id="74757-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74757-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="74757-116">Relationships</span></span>
<span data-ttu-id="74757-117">Keine</span><span class="sxs-lookup"><span data-stu-id="74757-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="74757-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="74757-118">JSON Representation</span></span>
<span data-ttu-id="74757-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="74757-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```





