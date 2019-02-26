---
title: deviceActionResult-Ressourcentyp
description: Ergebnis von Geräteaktion
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d08b4285f81c7b6f7e4962c4738279f84ba37b7d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261047"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="9e0f2-103">deviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9e0f2-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="9e0f2-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9e0f2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e0f2-105">Ergebnis von Gerätevorgang</span><span class="sxs-lookup"><span data-stu-id="9e0f2-105">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="9e0f2-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9e0f2-106">Properties</span></span>
|<span data-ttu-id="9e0f2-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9e0f2-107">Property</span></span>|<span data-ttu-id="9e0f2-108">Typ</span><span class="sxs-lookup"><span data-stu-id="9e0f2-108">Type</span></span>|<span data-ttu-id="9e0f2-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9e0f2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e0f2-110">actionName</span><span class="sxs-lookup"><span data-stu-id="9e0f2-110">actionName</span></span>|<span data-ttu-id="9e0f2-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9e0f2-111">String</span></span>|<span data-ttu-id="9e0f2-112">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="9e0f2-112">Action name</span></span>|
|<span data-ttu-id="9e0f2-113">actionState</span><span class="sxs-lookup"><span data-stu-id="9e0f2-113">actionState</span></span>|[<span data-ttu-id="9e0f2-114">actionState</span><span class="sxs-lookup"><span data-stu-id="9e0f2-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="9e0f2-115">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="9e0f2-115">State of the action.</span></span> <span data-ttu-id="9e0f2-116">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9e0f2-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9e0f2-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9e0f2-117">startDateTime</span></span>|<span data-ttu-id="9e0f2-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e0f2-118">DateTimeOffset</span></span>|<span data-ttu-id="9e0f2-119">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="9e0f2-119">Time the action was initiated</span></span>|
|<span data-ttu-id="9e0f2-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e0f2-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="9e0f2-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e0f2-121">DateTimeOffset</span></span>|<span data-ttu-id="9e0f2-122">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="9e0f2-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e0f2-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9e0f2-123">Relationships</span></span>
<span data-ttu-id="9e0f2-124">Keine</span><span class="sxs-lookup"><span data-stu-id="9e0f2-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e0f2-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9e0f2-125">JSON Representation</span></span>
<span data-ttu-id="9e0f2-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9e0f2-126">Here is a JSON representation of the resource.</span></span>
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



