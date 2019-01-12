---
title: configurationManagerClientEnabledFeatures-Ressourcentyp
description: Im Konfigurations-Manager-Client aktivierte Features
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 07b143a8d61335c44c83d1d88b9a67d2d3c2e4dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962086"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="d5639-103">configurationManagerClientEnabledFeatures-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d5639-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="d5639-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d5639-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5639-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d5639-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5639-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d5639-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5639-107">Im Konfigurations-Manager-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="d5639-107">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="d5639-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d5639-108">Properties</span></span>
|<span data-ttu-id="d5639-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d5639-109">Property</span></span>|<span data-ttu-id="d5639-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d5639-110">Type</span></span>|<span data-ttu-id="d5639-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5639-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5639-112">inventory</span><span class="sxs-lookup"><span data-stu-id="d5639-112">inventory</span></span>|<span data-ttu-id="d5639-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5639-113">Boolean</span></span>|<span data-ttu-id="d5639-114">Gibt an, ob der Bestand von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="d5639-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="d5639-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="d5639-115">modernApps</span></span>|<span data-ttu-id="d5639-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5639-116">Boolean</span></span>|<span data-ttu-id="d5639-117">Gibt an, ob die moderne Anwendung von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="d5639-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="d5639-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="d5639-118">resourceAccess</span></span>|<span data-ttu-id="d5639-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5639-119">Boolean</span></span>|<span data-ttu-id="d5639-120">Gibt an, ob der Zugriff auf Ressourcen von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="d5639-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="d5639-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5639-121">deviceConfiguration</span></span>|<span data-ttu-id="d5639-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5639-122">Boolean</span></span>|<span data-ttu-id="d5639-123">Gibt an, ob die Gerätekonfiguration von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="d5639-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="d5639-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="d5639-124">compliancePolicy</span></span>|<span data-ttu-id="d5639-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5639-125">Boolean</span></span>|<span data-ttu-id="d5639-126">Gibt an, ob Compliance-Richtlinie von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="d5639-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="d5639-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="d5639-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="d5639-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="d5639-128">Boolean</span></span>|<span data-ttu-id="d5639-129">Gibt an, ob Windows Update for Business von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="d5639-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5639-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d5639-130">Relationships</span></span>
<span data-ttu-id="d5639-131">Keine</span><span class="sxs-lookup"><span data-stu-id="d5639-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d5639-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d5639-132">JSON Representation</span></span>
<span data-ttu-id="d5639-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d5639-133">Here is a JSON representation of the resource.</span></span>
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





