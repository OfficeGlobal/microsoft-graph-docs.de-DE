---
title: managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp
description: Zusammenfassung der Richtlinienbereitstellung pro App
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 211b40c397ec7e3fb4000c8f4459056edec2a6f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972201"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="c3dbd-103">managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c3dbd-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="c3dbd-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c3dbd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3dbd-105">Zusammenfassung der Richtlinienbereitstellung pro App</span><span class="sxs-lookup"><span data-stu-id="c3dbd-105">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="c3dbd-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c3dbd-106">Properties</span></span>
|<span data-ttu-id="c3dbd-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c3dbd-107">Property</span></span>|<span data-ttu-id="c3dbd-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c3dbd-108">Type</span></span>|<span data-ttu-id="c3dbd-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3dbd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3dbd-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c3dbd-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="c3dbd-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c3dbd-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c3dbd-112">Bereitstellung einer App</span><span class="sxs-lookup"><span data-stu-id="c3dbd-112">Deployment of an app.</span></span>|
|<span data-ttu-id="c3dbd-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="c3dbd-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="c3dbd-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c3dbd-114">Int32</span></span>|<span data-ttu-id="c3dbd-115">Die Anzahl der Benutzer, auf die die Richtlinie angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="c3dbd-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3dbd-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c3dbd-116">Relationships</span></span>
<span data-ttu-id="c3dbd-117">Keine</span><span class="sxs-lookup"><span data-stu-id="c3dbd-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c3dbd-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c3dbd-118">JSON Representation</span></span>
<span data-ttu-id="c3dbd-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c3dbd-119">Here is a JSON representation of the resource.</span></span>
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



