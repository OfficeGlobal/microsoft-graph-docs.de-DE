---
title: managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp
description: Zusammenfassung der Richtlinienbereitstellung pro App
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 23966e2017780d3dcfde592d7159576403fe3192
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829750"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="185b8-103">managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="185b8-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="185b8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="185b8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="185b8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="185b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="185b8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="185b8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="185b8-107">Zusammenfassung der Richtlinienbereitstellung pro App</span><span class="sxs-lookup"><span data-stu-id="185b8-107">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="185b8-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="185b8-108">Properties</span></span>
|<span data-ttu-id="185b8-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="185b8-109">Property</span></span>|<span data-ttu-id="185b8-110">Typ</span><span class="sxs-lookup"><span data-stu-id="185b8-110">Type</span></span>|<span data-ttu-id="185b8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="185b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="185b8-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="185b8-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="185b8-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="185b8-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="185b8-114">Bereitstellung einer App</span><span class="sxs-lookup"><span data-stu-id="185b8-114">Deployment of an app.</span></span>|
|<span data-ttu-id="185b8-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="185b8-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="185b8-116">Int32</span><span class="sxs-lookup"><span data-stu-id="185b8-116">Int32</span></span>|<span data-ttu-id="185b8-117">Die Anzahl der Benutzer, auf die die Richtlinie angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="185b8-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="185b8-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="185b8-118">Relationships</span></span>
<span data-ttu-id="185b8-119">Keine</span><span class="sxs-lookup"><span data-stu-id="185b8-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="185b8-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="185b8-120">JSON Representation</span></span>
<span data-ttu-id="185b8-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="185b8-121">Here is a JSON representation of the resource.</span></span>
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





