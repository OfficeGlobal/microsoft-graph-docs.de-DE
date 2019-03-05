---
title: iosHomeScreenItem-Ressourcentyp
description: Stellt ein Element auf dem iOS-Startbildschirm dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8aecb99c036d3e8a5d89271afd6042ccb18b4fda
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253393"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="8a1b6-103">iosHomeScreenItem-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8a1b6-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="8a1b6-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8a1b6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a1b6-105">Stellt ein Element auf dem iOS-Startbildschirm dar.</span><span class="sxs-lookup"><span data-stu-id="8a1b6-105">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="8a1b6-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8a1b6-106">Properties</span></span>
|<span data-ttu-id="8a1b6-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8a1b6-107">Property</span></span>|<span data-ttu-id="8a1b6-108">Typ</span><span class="sxs-lookup"><span data-stu-id="8a1b6-108">Type</span></span>|<span data-ttu-id="8a1b6-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a1b6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a1b6-110">displayName</span><span class="sxs-lookup"><span data-stu-id="8a1b6-110">displayName</span></span>|<span data-ttu-id="8a1b6-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8a1b6-111">String</span></span>|<span data-ttu-id="8a1b6-112">Name der App</span><span class="sxs-lookup"><span data-stu-id="8a1b6-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a1b6-113">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8a1b6-113">Relationships</span></span>
<span data-ttu-id="8a1b6-114">Keine</span><span class="sxs-lookup"><span data-stu-id="8a1b6-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a1b6-115">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8a1b6-115">JSON Representation</span></span>
<span data-ttu-id="8a1b6-116">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8a1b6-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```



