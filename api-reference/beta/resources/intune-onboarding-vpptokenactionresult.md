---
title: Ressourcentyp vppTokenActionResult
description: Der Status der Aktion, die mit einem Apple Volume Purchase Program Token ausgeführt werden.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2fb78ea991ed43bd100a424ea7ddd7e23b22412d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414291"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="1aa7b-103">Ressourcentyp vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="1aa7b-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="1aa7b-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1aa7b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1aa7b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1aa7b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1aa7b-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1aa7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aa7b-107">Der Status der Aktion, die mit einem Apple Volume Purchase Program Token ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="1aa7b-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>

## <a name="properties"></a><span data-ttu-id="1aa7b-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1aa7b-108">Properties</span></span>
|<span data-ttu-id="1aa7b-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1aa7b-109">Property</span></span>|<span data-ttu-id="1aa7b-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1aa7b-110">Type</span></span>|<span data-ttu-id="1aa7b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1aa7b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aa7b-112">actionName</span><span class="sxs-lookup"><span data-stu-id="1aa7b-112">actionName</span></span>|<span data-ttu-id="1aa7b-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1aa7b-113">String</span></span>|<span data-ttu-id="1aa7b-114">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="1aa7b-114">Action name</span></span>|
|<span data-ttu-id="1aa7b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="1aa7b-115">actionState</span></span>|[<span data-ttu-id="1aa7b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="1aa7b-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="1aa7b-117">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="1aa7b-117">State of the action.</span></span> <span data-ttu-id="1aa7b-118">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="1aa7b-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="1aa7b-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="1aa7b-119">startDateTime</span></span>|<span data-ttu-id="1aa7b-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aa7b-120">DateTimeOffset</span></span>|<span data-ttu-id="1aa7b-121">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="1aa7b-121">Time the action was initiated</span></span>|
|<span data-ttu-id="1aa7b-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1aa7b-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="1aa7b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aa7b-123">DateTimeOffset</span></span>|<span data-ttu-id="1aa7b-124">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="1aa7b-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aa7b-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1aa7b-125">Relationships</span></span>
<span data-ttu-id="1aa7b-126">Keine</span><span class="sxs-lookup"><span data-stu-id="1aa7b-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1aa7b-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1aa7b-127">JSON Representation</span></span>
<span data-ttu-id="1aa7b-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1aa7b-128">Here is a JSON representation of the resource.</span></span>
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




