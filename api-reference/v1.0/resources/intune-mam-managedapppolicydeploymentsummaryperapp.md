---
title: managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp
description: Zusammenfassung der Richtlinienbereitstellung pro App
author: tfitzmac
ms.openlocfilehash: 95c05696f6c080f90b9de61c309a577924e599b1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354341"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="f2e66-103">managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f2e66-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="f2e66-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f2e66-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2e66-105">Zusammenfassung der Richtlinienbereitstellung pro App</span><span class="sxs-lookup"><span data-stu-id="f2e66-105">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="f2e66-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f2e66-106">Properties</span></span>
|<span data-ttu-id="f2e66-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f2e66-107">Property</span></span>|<span data-ttu-id="f2e66-108">Typ</span><span class="sxs-lookup"><span data-stu-id="f2e66-108">Type</span></span>|<span data-ttu-id="f2e66-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f2e66-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2e66-110">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2e66-110">mobileAppIdentifier</span></span>|[<span data-ttu-id="f2e66-111">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2e66-111">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="f2e66-112">Bereitstellung einer App</span><span class="sxs-lookup"><span data-stu-id="f2e66-112">Deployment of an app.</span></span>|
|<span data-ttu-id="f2e66-113">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="f2e66-113">configurationAppliedUserCount</span></span>|<span data-ttu-id="f2e66-114">Int32</span><span class="sxs-lookup"><span data-stu-id="f2e66-114">Int32</span></span>|<span data-ttu-id="f2e66-115">Die Anzahl der Benutzer, auf die die Richtlinie angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="f2e66-115">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2e66-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f2e66-116">Relationships</span></span>
<span data-ttu-id="f2e66-117">Keine</span><span class="sxs-lookup"><span data-stu-id="f2e66-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f2e66-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f2e66-118">JSON Representation</span></span>
<span data-ttu-id="f2e66-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f2e66-119">Here is a JSON representation of the resource.</span></span>
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



