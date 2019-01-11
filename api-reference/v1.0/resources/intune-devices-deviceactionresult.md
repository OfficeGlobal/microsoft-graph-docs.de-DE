---
title: deviceActionResult-Ressourcentyp
description: Ergebnis von Gerätevorgang
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1b802d1b09fbe65e9e1e72e4c34a387462e12113
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861124"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="ada76-103">deviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ada76-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="ada76-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ada76-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ada76-105">Ergebnis von Gerätevorgang</span><span class="sxs-lookup"><span data-stu-id="ada76-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="ada76-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ada76-106">Properties</span></span>
|<span data-ttu-id="ada76-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ada76-107">Property</span></span>|<span data-ttu-id="ada76-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ada76-108">Type</span></span>|<span data-ttu-id="ada76-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ada76-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ada76-110">actionName</span><span class="sxs-lookup"><span data-stu-id="ada76-110">actionName</span></span>|<span data-ttu-id="ada76-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ada76-111">String</span></span>|<span data-ttu-id="ada76-112">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="ada76-112">Action name</span></span>|
|<span data-ttu-id="ada76-113">actionState</span><span class="sxs-lookup"><span data-stu-id="ada76-113">actionState</span></span>|[<span data-ttu-id="ada76-114">actionState</span><span class="sxs-lookup"><span data-stu-id="ada76-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="ada76-115">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="ada76-115">State of the action.</span></span> <span data-ttu-id="ada76-116">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="ada76-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="ada76-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ada76-117">startDateTime</span></span>|<span data-ttu-id="ada76-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ada76-118">DateTimeOffset</span></span>|<span data-ttu-id="ada76-119">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="ada76-119">Time the action was initiated</span></span>|
|<span data-ttu-id="ada76-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ada76-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="ada76-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ada76-121">DateTimeOffset</span></span>|<span data-ttu-id="ada76-122">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="ada76-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="ada76-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ada76-123">Relationships</span></span>
<span data-ttu-id="ada76-124">Keine</span><span class="sxs-lookup"><span data-stu-id="ada76-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ada76-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ada76-125">JSON Representation</span></span>
<span data-ttu-id="ada76-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ada76-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```



