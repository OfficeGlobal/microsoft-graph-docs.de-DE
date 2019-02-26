---
title: updateWindowsDeviceAccountActionParameter-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d67599dfc9db2afa337324e3f1ba9334134458f4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256672"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="9d705-103">updateWindowsDeviceAccountActionParameter-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9d705-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="9d705-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9d705-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d705-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9d705-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9d705-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9d705-106">Properties</span></span>
|<span data-ttu-id="9d705-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9d705-107">Property</span></span>|<span data-ttu-id="9d705-108">Typ</span><span class="sxs-lookup"><span data-stu-id="9d705-108">Type</span></span>|<span data-ttu-id="9d705-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d705-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d705-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="9d705-110">deviceAccount</span></span>|[<span data-ttu-id="9d705-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="9d705-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="9d705-112">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9d705-112">Not yet documented</span></span>|
|<span data-ttu-id="9d705-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="9d705-113">passwordRotationEnabled</span></span>|<span data-ttu-id="9d705-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d705-114">Boolean</span></span>|<span data-ttu-id="9d705-115">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9d705-115">Not yet documented</span></span>|
|<span data-ttu-id="9d705-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="9d705-116">calendarSyncEnabled</span></span>|<span data-ttu-id="9d705-117">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9d705-117">Boolean</span></span>|<span data-ttu-id="9d705-118">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9d705-118">Not yet documented</span></span>|
|<span data-ttu-id="9d705-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="9d705-119">deviceAccountEmail</span></span>|<span data-ttu-id="9d705-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9d705-120">String</span></span>|<span data-ttu-id="9d705-121">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9d705-121">Not yet documented</span></span>|
|<span data-ttu-id="9d705-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="9d705-122">exchangeServer</span></span>|<span data-ttu-id="9d705-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9d705-123">String</span></span>|<span data-ttu-id="9d705-124">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="9d705-124">Not yet documented</span></span>|
|<span data-ttu-id="9d705-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="9d705-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="9d705-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9d705-126">String</span></span>|<span data-ttu-id="9d705-127">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="9d705-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d705-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9d705-128">Relationships</span></span>
<span data-ttu-id="9d705-129">Keine</span><span class="sxs-lookup"><span data-stu-id="9d705-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d705-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9d705-130">JSON Representation</span></span>
<span data-ttu-id="9d705-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9d705-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```



