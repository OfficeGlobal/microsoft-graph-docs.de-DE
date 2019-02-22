---
title: vppTokenActionResult-Ressourcentyp
description: Der Status der Aktion, die mit einem Apple Volume Purchase Program-Token ausgeführt wurde.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 853c5c12ca0a85fe0f5a16efa86321e46a28ec5c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159388"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="bac36-103">vppTokenActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bac36-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="bac36-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bac36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bac36-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bac36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bac36-106">Der Status der Aktion, die mit einem Apple Volume Purchase Program-Token ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="bac36-106">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="bac36-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bac36-107">Properties</span></span>
|<span data-ttu-id="bac36-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bac36-108">Property</span></span>|<span data-ttu-id="bac36-109">Typ</span><span class="sxs-lookup"><span data-stu-id="bac36-109">Type</span></span>|<span data-ttu-id="bac36-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bac36-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bac36-111">actionName</span><span class="sxs-lookup"><span data-stu-id="bac36-111">actionName</span></span>|<span data-ttu-id="bac36-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bac36-112">String</span></span>|<span data-ttu-id="bac36-113">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="bac36-113">Action name</span></span>|
|<span data-ttu-id="bac36-114">actionState</span><span class="sxs-lookup"><span data-stu-id="bac36-114">actionState</span></span>|[<span data-ttu-id="bac36-115">actionState</span><span class="sxs-lookup"><span data-stu-id="bac36-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="bac36-116">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="bac36-116">State of the action.</span></span> <span data-ttu-id="bac36-117">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="bac36-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="bac36-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bac36-118">startDateTime</span></span>|<span data-ttu-id="bac36-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bac36-119">DateTimeOffset</span></span>|<span data-ttu-id="bac36-120">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="bac36-120">Time the action was initiated</span></span>|
|<span data-ttu-id="bac36-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="bac36-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="bac36-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bac36-122">DateTimeOffset</span></span>|<span data-ttu-id="bac36-123">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="bac36-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="bac36-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bac36-124">Relationships</span></span>
<span data-ttu-id="bac36-125">Keine</span><span class="sxs-lookup"><span data-stu-id="bac36-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bac36-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bac36-126">JSON Representation</span></span>
<span data-ttu-id="bac36-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bac36-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




