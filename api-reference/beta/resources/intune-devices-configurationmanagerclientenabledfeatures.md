---
title: configurationManagerClientEnabledFeatures-Ressourcentyp
description: Im Konfigurations-Manager-Client aktivierte Features
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed376bc616c26f1ad6e8a3ea06d3898c051e8d0b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148776"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="8a1eb-103">configurationManagerClientEnabledFeatures-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8a1eb-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="8a1eb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8a1eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a1eb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8a1eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a1eb-106">Im Konfigurations-Manager-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="8a1eb-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="8a1eb-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8a1eb-107">Properties</span></span>
|<span data-ttu-id="8a1eb-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8a1eb-108">Property</span></span>|<span data-ttu-id="8a1eb-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8a1eb-109">Type</span></span>|<span data-ttu-id="8a1eb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8a1eb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a1eb-111">inventory</span><span class="sxs-lookup"><span data-stu-id="8a1eb-111">inventory</span></span>|<span data-ttu-id="8a1eb-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a1eb-112">Boolean</span></span>|<span data-ttu-id="8a1eb-113">Gibt an, ob der Bestand von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="8a1eb-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="8a1eb-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="8a1eb-114">modernApps</span></span>|<span data-ttu-id="8a1eb-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a1eb-115">Boolean</span></span>|<span data-ttu-id="8a1eb-116">Gibt an, ob die moderne Anwendung von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="8a1eb-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="8a1eb-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="8a1eb-117">resourceAccess</span></span>|<span data-ttu-id="8a1eb-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a1eb-118">Boolean</span></span>|<span data-ttu-id="8a1eb-119">Gibt an, ob der Zugriff auf Ressourcen von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="8a1eb-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="8a1eb-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a1eb-120">deviceConfiguration</span></span>|<span data-ttu-id="8a1eb-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a1eb-121">Boolean</span></span>|<span data-ttu-id="8a1eb-122">Gibt an, ob die Gerätekonfiguration von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="8a1eb-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="8a1eb-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="8a1eb-123">compliancePolicy</span></span>|<span data-ttu-id="8a1eb-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a1eb-124">Boolean</span></span>|<span data-ttu-id="8a1eb-125">Gibt an, ob Compliance-Richtlinie von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="8a1eb-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="8a1eb-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="8a1eb-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="8a1eb-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a1eb-127">Boolean</span></span>|<span data-ttu-id="8a1eb-128">Gibt an, ob Windows Update for Business von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="8a1eb-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="8a1eb-129">endpointProtection</span><span class="sxs-lookup"><span data-stu-id="8a1eb-129">endpointProtection</span></span>|<span data-ttu-id="8a1eb-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a1eb-130">Boolean</span></span>|<span data-ttu-id="8a1eb-131">Ob der Endpunktschutz von InTune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="8a1eb-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="8a1eb-132">officeApps</span><span class="sxs-lookup"><span data-stu-id="8a1eb-132">officeApps</span></span>|<span data-ttu-id="8a1eb-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a1eb-133">Boolean</span></span>|<span data-ttu-id="8a1eb-134">Ob die Office-Anwendung von InTune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="8a1eb-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a1eb-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8a1eb-135">Relationships</span></span>
<span data-ttu-id="8a1eb-136">Keine</span><span class="sxs-lookup"><span data-stu-id="8a1eb-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a1eb-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8a1eb-137">JSON Representation</span></span>
<span data-ttu-id="8a1eb-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8a1eb-138">Here is a JSON representation of the resource.</span></span>
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
  "windowsUpdateForBusiness": true,
  "endpointProtection": true,
  "officeApps": true
}
```




