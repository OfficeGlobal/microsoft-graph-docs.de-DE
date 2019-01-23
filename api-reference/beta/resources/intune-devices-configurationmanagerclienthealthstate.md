---
title: Ressourcentyp configurationManagerClientHealthState
description: Konfigurations-Manager-Client-Zustand
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55ba2b24df0d1d4c278f4785a310237c9c32cd9b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425827"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="729f3-103">Ressourcentyp configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="729f3-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="729f3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="729f3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="729f3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="729f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="729f3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="729f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="729f3-107">Konfigurations-Manager-Client-Zustand</span><span class="sxs-lookup"><span data-stu-id="729f3-107">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="729f3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="729f3-108">Properties</span></span>
|<span data-ttu-id="729f3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="729f3-109">Property</span></span>|<span data-ttu-id="729f3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="729f3-110">Type</span></span>|<span data-ttu-id="729f3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="729f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="729f3-112">state</span><span class="sxs-lookup"><span data-stu-id="729f3-112">state</span></span>|[<span data-ttu-id="729f3-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="729f3-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="729f3-114">Aktuelle Configuration Manager-Client-Zustand.</span><span class="sxs-lookup"><span data-stu-id="729f3-114">Current configuration manager client state.</span></span> <span data-ttu-id="729f3-115">Mögliche Werte sind: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed` und `communicationError`.</span><span class="sxs-lookup"><span data-stu-id="729f3-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="729f3-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="729f3-116">errorCode</span></span>|<span data-ttu-id="729f3-117">Int32</span><span class="sxs-lookup"><span data-stu-id="729f3-117">Int32</span></span>|<span data-ttu-id="729f3-118">Der Fehlercode für ausgefallenen Zustand.</span><span class="sxs-lookup"><span data-stu-id="729f3-118">Error code for failed state.</span></span>|
|<span data-ttu-id="729f3-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="729f3-119">lastSyncDateTime</span></span>|<span data-ttu-id="729f3-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="729f3-120">DateTimeOffset</span></span>|<span data-ttu-id="729f3-121">Zeigen Sie DateTime fo letzte Synchronisierung mit Configuration Manager-Management.</span><span class="sxs-lookup"><span data-stu-id="729f3-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="729f3-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="729f3-122">Relationships</span></span>
<span data-ttu-id="729f3-123">Keine</span><span class="sxs-lookup"><span data-stu-id="729f3-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="729f3-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="729f3-124">JSON Representation</span></span>
<span data-ttu-id="729f3-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="729f3-125">Here is a JSON representation of the resource.</span></span>
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




