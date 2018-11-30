---
title: deviceActionResult-Ressourcentyp
description: Ergebnis von Gerätevorgang
ms.openlocfilehash: 9d7804b994474778f0f06c52079e09ed5887a09f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018814"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="308af-103">deviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="308af-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="308af-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="308af-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="308af-105">Ergebnis von Gerätevorgang</span><span class="sxs-lookup"><span data-stu-id="308af-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="308af-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="308af-106">Properties</span></span>
|<span data-ttu-id="308af-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="308af-107">Property</span></span>|<span data-ttu-id="308af-108">Typ</span><span class="sxs-lookup"><span data-stu-id="308af-108">Type</span></span>|<span data-ttu-id="308af-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="308af-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="308af-110">actionName</span><span class="sxs-lookup"><span data-stu-id="308af-110">actionName</span></span>|<span data-ttu-id="308af-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="308af-111">String</span></span>|<span data-ttu-id="308af-112">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="308af-112">Action name</span></span>|
|<span data-ttu-id="308af-113">actionState</span><span class="sxs-lookup"><span data-stu-id="308af-113">actionState</span></span>|[<span data-ttu-id="308af-114">actionState</span><span class="sxs-lookup"><span data-stu-id="308af-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="308af-115">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="308af-115">State of the action.</span></span> <span data-ttu-id="308af-116">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="308af-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="308af-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="308af-117">startDateTime</span></span>|<span data-ttu-id="308af-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="308af-118">DateTimeOffset</span></span>|<span data-ttu-id="308af-119">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="308af-119">Time the action was initiated</span></span>|
|<span data-ttu-id="308af-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="308af-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="308af-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="308af-121">DateTimeOffset</span></span>|<span data-ttu-id="308af-122">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="308af-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="308af-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="308af-123">Relationships</span></span>
<span data-ttu-id="308af-124">Keine</span><span class="sxs-lookup"><span data-stu-id="308af-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="308af-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="308af-125">JSON Representation</span></span>
<span data-ttu-id="308af-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="308af-126">Here is a JSON representation of the resource.</span></span>
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



