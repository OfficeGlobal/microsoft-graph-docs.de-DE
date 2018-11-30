---
title: configurationManagerClientEnabledFeatures-Ressourcentyp
description: Im Konfigurations-Manager-Client aktivierte Features
ms.openlocfilehash: 54d5d40a50b2946fec1c69c619dc76bec1f32502
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018812"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="e2cd3-103">configurationManagerClientEnabledFeatures-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e2cd3-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="e2cd3-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e2cd3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2cd3-105">Im Konfigurations-Manager-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="e2cd3-105">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="e2cd3-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e2cd3-106">Properties</span></span>
|<span data-ttu-id="e2cd3-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2cd3-107">Property</span></span>|<span data-ttu-id="e2cd3-108">Typ</span><span class="sxs-lookup"><span data-stu-id="e2cd3-108">Type</span></span>|<span data-ttu-id="e2cd3-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2cd3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2cd3-110">inventory</span><span class="sxs-lookup"><span data-stu-id="e2cd3-110">inventory</span></span>|<span data-ttu-id="e2cd3-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cd3-111">Boolean</span></span>|<span data-ttu-id="e2cd3-112">Gibt an, ob der Bestand von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="e2cd3-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="e2cd3-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="e2cd3-113">modernApps</span></span>|<span data-ttu-id="e2cd3-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cd3-114">Boolean</span></span>|<span data-ttu-id="e2cd3-115">Gibt an, ob die moderne Anwendung von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="e2cd3-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="e2cd3-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="e2cd3-116">resourceAccess</span></span>|<span data-ttu-id="e2cd3-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cd3-117">Boolean</span></span>|<span data-ttu-id="e2cd3-118">Gibt an, ob der Zugriff auf Ressourcen von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="e2cd3-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="e2cd3-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2cd3-119">deviceConfiguration</span></span>|<span data-ttu-id="e2cd3-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cd3-120">Boolean</span></span>|<span data-ttu-id="e2cd3-121">Gibt an, ob die Gerätekonfiguration von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="e2cd3-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="e2cd3-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e2cd3-122">compliancePolicy</span></span>|<span data-ttu-id="e2cd3-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cd3-123">Boolean</span></span>|<span data-ttu-id="e2cd3-124">Gibt an, ob Compliance-Richtlinie von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="e2cd3-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="e2cd3-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="e2cd3-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="e2cd3-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2cd3-126">Boolean</span></span>|<span data-ttu-id="e2cd3-127">Gibt an, ob Windows Update for Business von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="e2cd3-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2cd3-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e2cd3-128">Relationships</span></span>
<span data-ttu-id="e2cd3-129">Keine</span><span class="sxs-lookup"><span data-stu-id="e2cd3-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2cd3-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e2cd3-130">JSON Representation</span></span>
<span data-ttu-id="e2cd3-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e2cd3-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```



