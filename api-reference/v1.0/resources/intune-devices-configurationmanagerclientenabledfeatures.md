---
title: configurationManagerClientEnabledFeatures-Ressourcentyp
description: Im Konfigurations-Manager-Client aktivierte Features
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91ffd0180660b33e9ead5210f9b23870af18e29a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264421"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="3d374-103">configurationManagerClientEnabledFeatures-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3d374-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="3d374-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3d374-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d374-105">Im Konfigurations-Manager-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="3d374-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="3d374-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3d374-106">Properties</span></span>
|<span data-ttu-id="3d374-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d374-107">Property</span></span>|<span data-ttu-id="3d374-108">Typ</span><span class="sxs-lookup"><span data-stu-id="3d374-108">Type</span></span>|<span data-ttu-id="3d374-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d374-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d374-110">inventory</span><span class="sxs-lookup"><span data-stu-id="3d374-110">inventory</span></span>|<span data-ttu-id="3d374-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d374-111">Boolean</span></span>|<span data-ttu-id="3d374-112">Gibt an, ob der Bestand von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="3d374-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="3d374-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="3d374-113">modernApps</span></span>|<span data-ttu-id="3d374-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d374-114">Boolean</span></span>|<span data-ttu-id="3d374-115">Gibt an, ob die moderne Anwendung von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="3d374-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="3d374-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="3d374-116">resourceAccess</span></span>|<span data-ttu-id="3d374-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d374-117">Boolean</span></span>|<span data-ttu-id="3d374-118">Gibt an, ob der Zugriff auf Ressourcen von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="3d374-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="3d374-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3d374-119">deviceConfiguration</span></span>|<span data-ttu-id="3d374-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d374-120">Boolean</span></span>|<span data-ttu-id="3d374-121">Gibt an, ob die Gerätekonfiguration von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="3d374-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="3d374-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3d374-122">compliancePolicy</span></span>|<span data-ttu-id="3d374-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d374-123">Boolean</span></span>|<span data-ttu-id="3d374-124">Gibt an, ob Compliance-Richtlinie von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="3d374-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="3d374-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="3d374-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="3d374-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d374-126">Boolean</span></span>|<span data-ttu-id="3d374-127">Gibt an, ob Windows Update for Business von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="3d374-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d374-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3d374-128">Relationships</span></span>
<span data-ttu-id="3d374-129">Keine</span><span class="sxs-lookup"><span data-stu-id="3d374-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d374-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3d374-130">JSON Representation</span></span>
<span data-ttu-id="3d374-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3d374-131">Here is a JSON representation of the resource.</span></span>
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



