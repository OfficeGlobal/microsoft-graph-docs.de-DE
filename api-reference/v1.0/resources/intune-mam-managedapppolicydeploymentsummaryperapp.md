---
title: managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp
description: Zusammenfassung der Richtlinienbereitstellung pro App
ms.openlocfilehash: 56b7952049c6ad41ee46f6b77c821aa32b1c4de8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018976"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="5d08b-103">managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5d08b-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="5d08b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5d08b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d08b-105">Zusammenfassung der Richtlinienbereitstellung pro App</span><span class="sxs-lookup"><span data-stu-id="5d08b-105">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="5d08b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5d08b-106">Properties</span></span>
|<span data-ttu-id="5d08b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5d08b-107">Property</span></span>|<span data-ttu-id="5d08b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="5d08b-108">Type</span></span>|<span data-ttu-id="5d08b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5d08b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d08b-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5d08b-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="5d08b-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="5d08b-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="5d08b-112">Bereitstellung einer App</span><span class="sxs-lookup"><span data-stu-id="5d08b-112">Deployment of an app.</span></span>|
|<span data-ttu-id="5d08b-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="5d08b-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="5d08b-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5d08b-114">Int32</span></span>|<span data-ttu-id="5d08b-115">Die Anzahl der Benutzer, auf die die Richtlinie angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="5d08b-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d08b-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5d08b-116">Relationships</span></span>
<span data-ttu-id="5d08b-117">Keine</span><span class="sxs-lookup"><span data-stu-id="5d08b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5d08b-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5d08b-118">JSON Representation</span></span>
<span data-ttu-id="5d08b-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5d08b-119">Here is a JSON representation of the resource.</span></span>
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



