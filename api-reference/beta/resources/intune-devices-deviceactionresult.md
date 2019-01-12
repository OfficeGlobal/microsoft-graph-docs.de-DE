---
title: deviceActionResult-Ressourcentyp
description: Ergebnis von Gerätevorgang
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 22fd8e1bc338191bba54ba9f655f03899054ae86
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912302"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="28539-103">deviceActionResult-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="28539-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="28539-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="28539-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28539-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28539-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28539-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="28539-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28539-107">Ergebnis von Gerätevorgang</span><span class="sxs-lookup"><span data-stu-id="28539-107">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="28539-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="28539-108">Properties</span></span>
|<span data-ttu-id="28539-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28539-109">Property</span></span>|<span data-ttu-id="28539-110">Typ</span><span class="sxs-lookup"><span data-stu-id="28539-110">Type</span></span>|<span data-ttu-id="28539-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28539-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28539-112">actionName</span><span class="sxs-lookup"><span data-stu-id="28539-112">actionName</span></span>|<span data-ttu-id="28539-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="28539-113">String</span></span>|<span data-ttu-id="28539-114">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="28539-114">Action name</span></span>|
|<span data-ttu-id="28539-115">actionState</span><span class="sxs-lookup"><span data-stu-id="28539-115">actionState</span></span>|[<span data-ttu-id="28539-116">actionState</span><span class="sxs-lookup"><span data-stu-id="28539-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="28539-117">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="28539-117">State of the action.</span></span> <span data-ttu-id="28539-118">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="28539-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="28539-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="28539-119">startDateTime</span></span>|<span data-ttu-id="28539-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28539-120">DateTimeOffset</span></span>|<span data-ttu-id="28539-121">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="28539-121">Time the action was initiated</span></span>|
|<span data-ttu-id="28539-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="28539-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="28539-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28539-123">DateTimeOffset</span></span>|<span data-ttu-id="28539-124">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="28539-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="28539-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="28539-125">Relationships</span></span>
<span data-ttu-id="28539-126">Keine</span><span class="sxs-lookup"><span data-stu-id="28539-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="28539-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="28539-127">JSON Representation</span></span>
<span data-ttu-id="28539-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="28539-128">Here is a JSON representation of the resource.</span></span>
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





