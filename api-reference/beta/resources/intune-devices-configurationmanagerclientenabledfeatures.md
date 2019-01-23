---
title: configurationManagerClientEnabledFeatures-Ressourcentyp
description: Im Konfigurations-Manager-Client aktivierte Features
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7975130bb047e097ea0d52a4ce770fb35e4efa32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425904"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="c8fb6-103">configurationManagerClientEnabledFeatures-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c8fb6-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="c8fb6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c8fb6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c8fb6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8fb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8fb6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c8fb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8fb6-107">Im Konfigurations-Manager-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="c8fb6-107">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="c8fb6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c8fb6-108">Properties</span></span>
|<span data-ttu-id="c8fb6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c8fb6-109">Property</span></span>|<span data-ttu-id="c8fb6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c8fb6-110">Type</span></span>|<span data-ttu-id="c8fb6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c8fb6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8fb6-112">inventory</span><span class="sxs-lookup"><span data-stu-id="c8fb6-112">inventory</span></span>|<span data-ttu-id="c8fb6-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8fb6-113">Boolean</span></span>|<span data-ttu-id="c8fb6-114">Gibt an, ob der Bestand von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="c8fb6-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="c8fb6-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="c8fb6-115">modernApps</span></span>|<span data-ttu-id="c8fb6-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8fb6-116">Boolean</span></span>|<span data-ttu-id="c8fb6-117">Gibt an, ob die moderne Anwendung von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="c8fb6-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="c8fb6-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="c8fb6-118">resourceAccess</span></span>|<span data-ttu-id="c8fb6-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8fb6-119">Boolean</span></span>|<span data-ttu-id="c8fb6-120">Gibt an, ob der Zugriff auf Ressourcen von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="c8fb6-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="c8fb6-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8fb6-121">deviceConfiguration</span></span>|<span data-ttu-id="c8fb6-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8fb6-122">Boolean</span></span>|<span data-ttu-id="c8fb6-123">Gibt an, ob die Gerätekonfiguration von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="c8fb6-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="c8fb6-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c8fb6-124">compliancePolicy</span></span>|<span data-ttu-id="c8fb6-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8fb6-125">Boolean</span></span>|<span data-ttu-id="c8fb6-126">Gibt an, ob Compliance-Richtlinie von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="c8fb6-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="c8fb6-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="c8fb6-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="c8fb6-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8fb6-128">Boolean</span></span>|<span data-ttu-id="c8fb6-129">Gibt an, ob Windows Update for Business von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="c8fb6-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8fb6-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c8fb6-130">Relationships</span></span>
<span data-ttu-id="c8fb6-131">Keine</span><span class="sxs-lookup"><span data-stu-id="c8fb6-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8fb6-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c8fb6-132">JSON Representation</span></span>
<span data-ttu-id="c8fb6-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c8fb6-133">Here is a JSON representation of the resource.</span></span>
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




