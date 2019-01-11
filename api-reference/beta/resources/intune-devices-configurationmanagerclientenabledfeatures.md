---
title: configurationManagerClientEnabledFeatures-Ressourcentyp
description: Im Konfigurations-Manager-Client aktivierte Features
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9517bb807ad257ddba94b991223b781e91bbbc68
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890090"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="98cee-103">configurationManagerClientEnabledFeatures-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="98cee-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="98cee-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="98cee-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98cee-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="98cee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98cee-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="98cee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98cee-107">Im Konfigurations-Manager-Client aktivierte Features</span><span class="sxs-lookup"><span data-stu-id="98cee-107">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="98cee-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="98cee-108">Properties</span></span>
|<span data-ttu-id="98cee-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="98cee-109">Property</span></span>|<span data-ttu-id="98cee-110">Typ</span><span class="sxs-lookup"><span data-stu-id="98cee-110">Type</span></span>|<span data-ttu-id="98cee-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98cee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98cee-112">inventory</span><span class="sxs-lookup"><span data-stu-id="98cee-112">inventory</span></span>|<span data-ttu-id="98cee-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="98cee-113">Boolean</span></span>|<span data-ttu-id="98cee-114">Gibt an, ob der Bestand von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="98cee-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="98cee-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="98cee-115">modernApps</span></span>|<span data-ttu-id="98cee-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="98cee-116">Boolean</span></span>|<span data-ttu-id="98cee-117">Gibt an, ob die moderne Anwendung von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="98cee-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="98cee-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="98cee-118">resourceAccess</span></span>|<span data-ttu-id="98cee-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="98cee-119">Boolean</span></span>|<span data-ttu-id="98cee-120">Gibt an, ob der Zugriff auf Ressourcen von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="98cee-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="98cee-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="98cee-121">deviceConfiguration</span></span>|<span data-ttu-id="98cee-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="98cee-122">Boolean</span></span>|<span data-ttu-id="98cee-123">Gibt an, ob die Gerätekonfiguration von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="98cee-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="98cee-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="98cee-124">compliancePolicy</span></span>|<span data-ttu-id="98cee-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="98cee-125">Boolean</span></span>|<span data-ttu-id="98cee-126">Gibt an, ob Compliance-Richtlinie von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="98cee-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="98cee-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="98cee-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="98cee-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="98cee-128">Boolean</span></span>|<span data-ttu-id="98cee-129">Gibt an, ob Windows Update for Business von Intune verwaltet wird</span><span class="sxs-lookup"><span data-stu-id="98cee-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="98cee-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="98cee-130">Relationships</span></span>
<span data-ttu-id="98cee-131">Keine</span><span class="sxs-lookup"><span data-stu-id="98cee-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98cee-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="98cee-132">JSON Representation</span></span>
<span data-ttu-id="98cee-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="98cee-133">Here is a JSON representation of the resource.</span></span>
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





