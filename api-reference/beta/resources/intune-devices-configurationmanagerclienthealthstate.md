---
title: Ressourcentyp configurationManagerClientHealthState
description: Konfigurations-Manager-Client-Zustand
author: tfitzmac
ms.openlocfilehash: 8361d74f675cf1eaf70b78e2350aae2fc6e83554
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302786"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="e3f7a-103">Ressourcentyp configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="e3f7a-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="e3f7a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="e3f7a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3f7a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e3f7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3f7a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e3f7a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3f7a-107">Konfigurations-Manager-Client-Zustand</span><span class="sxs-lookup"><span data-stu-id="e3f7a-107">Configuration manager client health state</span></span>
## <a name="properties"></a><span data-ttu-id="e3f7a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e3f7a-108">Properties</span></span>
|<span data-ttu-id="e3f7a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e3f7a-109">Property</span></span>|<span data-ttu-id="e3f7a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e3f7a-110">Type</span></span>|<span data-ttu-id="e3f7a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e3f7a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3f7a-112">state</span><span class="sxs-lookup"><span data-stu-id="e3f7a-112">state</span></span>|[<span data-ttu-id="e3f7a-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="e3f7a-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="e3f7a-114">Aktuelle Configuration Manager-Client-Zustand.</span><span class="sxs-lookup"><span data-stu-id="e3f7a-114">Current configuration manager client state.</span></span> <span data-ttu-id="e3f7a-115">Mögliche Werte sind: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed` und `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="e3f7a-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="e3f7a-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="e3f7a-116">errorCode</span></span>|<span data-ttu-id="e3f7a-117">Int32</span><span class="sxs-lookup"><span data-stu-id="e3f7a-117">Int32</span></span>|<span data-ttu-id="e3f7a-118">Der Fehlercode für ausgefallenen Zustand.</span><span class="sxs-lookup"><span data-stu-id="e3f7a-118">Error code for failed state.</span></span>|
|<span data-ttu-id="e3f7a-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e3f7a-119">lastSyncDateTime</span></span>|<span data-ttu-id="e3f7a-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3f7a-120">DateTimeOffset</span></span>|<span data-ttu-id="e3f7a-121">Zeigen Sie DateTime fo letzte Synchronisierung mit Configuration Manager-Management.</span><span class="sxs-lookup"><span data-stu-id="e3f7a-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3f7a-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e3f7a-122">Relationships</span></span>
<span data-ttu-id="e3f7a-123">Keine</span><span class="sxs-lookup"><span data-stu-id="e3f7a-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e3f7a-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e3f7a-124">JSON Representation</span></span>
<span data-ttu-id="e3f7a-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e3f7a-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```





