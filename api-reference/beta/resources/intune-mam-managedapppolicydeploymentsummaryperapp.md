---
title: managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp
description: Zusammenfassung der Richtlinienbereitstellung pro App
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d940a5cf996f2fa42ac73ccba89ccef7f5999e5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156973"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="0d396-103">managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0d396-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="0d396-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0d396-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d396-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0d396-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d396-106">Zusammenfassung der Richtlinienbereitstellung pro App</span><span class="sxs-lookup"><span data-stu-id="0d396-106">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="0d396-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0d396-107">Properties</span></span>
|<span data-ttu-id="0d396-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d396-108">Property</span></span>|<span data-ttu-id="0d396-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0d396-109">Type</span></span>|<span data-ttu-id="0d396-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d396-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d396-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="0d396-111">mobileAppIdentifier</span></span>|[<span data-ttu-id="0d396-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="0d396-112">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="0d396-113">Bereitstellung einer App</span><span class="sxs-lookup"><span data-stu-id="0d396-113">Deployment of an app.</span></span>|
|<span data-ttu-id="0d396-114">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="0d396-114">configurationAppliedUserCount</span></span>|<span data-ttu-id="0d396-115">Int32</span><span class="sxs-lookup"><span data-stu-id="0d396-115">Int32</span></span>|<span data-ttu-id="0d396-116">Die Anzahl der Benutzer, auf die die Richtlinie angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="0d396-116">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d396-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0d396-117">Relationships</span></span>
<span data-ttu-id="0d396-118">Keine</span><span class="sxs-lookup"><span data-stu-id="0d396-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d396-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0d396-119">JSON Representation</span></span>
<span data-ttu-id="0d396-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0d396-120">Here is a JSON representation of the resource.</span></span>
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




