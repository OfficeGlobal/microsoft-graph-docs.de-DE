---
title: Ressourcentyp vppTokenActionResult
description: Der Status der Aktion, die mit einem Apple Volume Purchase Program Token ausgeführt werden.
author: tfitzmac
ms.openlocfilehash: 0b8b074e879321d0aed361373c49e6ed1fd16e62
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341678"
---
# <a name="vpptokenactionresult-resource-type"></a><span data-ttu-id="090e5-103">Ressourcentyp vppTokenActionResult</span><span class="sxs-lookup"><span data-stu-id="090e5-103">vppTokenActionResult resource type</span></span>

> <span data-ttu-id="090e5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="090e5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="090e5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="090e5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="090e5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="090e5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="090e5-107">Der Status der Aktion, die mit einem Apple Volume Purchase Program Token ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="090e5-107">The status of the action performed with an Apple Volume Purchase Program token.</span></span>
## <a name="properties"></a><span data-ttu-id="090e5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="090e5-108">Properties</span></span>
|<span data-ttu-id="090e5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="090e5-109">Property</span></span>|<span data-ttu-id="090e5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="090e5-110">Type</span></span>|<span data-ttu-id="090e5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="090e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="090e5-112">actionName</span><span class="sxs-lookup"><span data-stu-id="090e5-112">actionName</span></span>|<span data-ttu-id="090e5-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="090e5-113">String</span></span>|<span data-ttu-id="090e5-114">Name der Aktion</span><span class="sxs-lookup"><span data-stu-id="090e5-114">Action name</span></span>|
|<span data-ttu-id="090e5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="090e5-115">actionState</span></span>|[<span data-ttu-id="090e5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="090e5-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="090e5-117">Status der Aktion.</span><span class="sxs-lookup"><span data-stu-id="090e5-117">State of the action.</span></span> <span data-ttu-id="090e5-118">Mögliche Werte sind: `none`, `pending`, `canceled`, `active`, `done`, `failed` und `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="090e5-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="090e5-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="090e5-119">startDateTime</span></span>|<span data-ttu-id="090e5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="090e5-120">DateTimeOffset</span></span>|<span data-ttu-id="090e5-121">Zeitpunkt der Einleitung der Aktion</span><span class="sxs-lookup"><span data-stu-id="090e5-121">Time the action was initiated</span></span>|
|<span data-ttu-id="090e5-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="090e5-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="090e5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="090e5-123">DateTimeOffset</span></span>|<span data-ttu-id="090e5-124">Zeitpunkt der letzten Aktualisierung des Aktionszustands</span><span class="sxs-lookup"><span data-stu-id="090e5-124">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="090e5-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="090e5-125">Relationships</span></span>
<span data-ttu-id="090e5-126">Keine</span><span class="sxs-lookup"><span data-stu-id="090e5-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="090e5-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="090e5-127">JSON Representation</span></span>
<span data-ttu-id="090e5-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="090e5-128">Here is a JSON representation of the resource.</span></span>
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





