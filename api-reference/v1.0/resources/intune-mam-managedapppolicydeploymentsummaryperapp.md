---
title: managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp
description: Zusammenfassung der Richtlinienbereitstellung pro App
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 149a578f60ba5953f77c83ca2fbc3810931dffff
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262510"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="695ea-103">managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="695ea-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="695ea-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="695ea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="695ea-105">Zusammenfassung der Richtlinienbereitstellung pro App</span><span class="sxs-lookup"><span data-stu-id="695ea-105">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="695ea-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="695ea-106">Properties</span></span>
|<span data-ttu-id="695ea-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="695ea-107">Property</span></span>|<span data-ttu-id="695ea-108">Typ</span><span class="sxs-lookup"><span data-stu-id="695ea-108">Type</span></span>|<span data-ttu-id="695ea-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="695ea-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="695ea-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="695ea-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="695ea-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="695ea-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="695ea-112">Bereitstellung einer App</span><span class="sxs-lookup"><span data-stu-id="695ea-112">Deployment of an app.</span></span>|
|<span data-ttu-id="695ea-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="695ea-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="695ea-114">Int32</span><span class="sxs-lookup"><span data-stu-id="695ea-114">Int32</span></span>|<span data-ttu-id="695ea-115">Die Anzahl der Benutzer, auf die die Richtlinie angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="695ea-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="695ea-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="695ea-116">Relationships</span></span>
<span data-ttu-id="695ea-117">Keine</span><span class="sxs-lookup"><span data-stu-id="695ea-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="695ea-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="695ea-118">JSON Representation</span></span>
<span data-ttu-id="695ea-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="695ea-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```



