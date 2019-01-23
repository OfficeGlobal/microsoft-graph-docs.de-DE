---
title: managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp
description: Zusammenfassung der Richtlinienbereitstellung pro App
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0e6053a1d690a68359fa30d5e5ac4c0ce5520bc6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411092"
---
# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="15ada-103">managedAppPolicyDeploymentSummaryPerApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="15ada-103">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="15ada-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="15ada-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="15ada-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15ada-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15ada-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="15ada-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15ada-107">Zusammenfassung der Richtlinienbereitstellung pro App</span><span class="sxs-lookup"><span data-stu-id="15ada-107">Represents policy deployment summary per app.</span></span>

## <a name="properties"></a><span data-ttu-id="15ada-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="15ada-108">Properties</span></span>
|<span data-ttu-id="15ada-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15ada-109">Property</span></span>|<span data-ttu-id="15ada-110">Typ</span><span class="sxs-lookup"><span data-stu-id="15ada-110">Type</span></span>|<span data-ttu-id="15ada-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15ada-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15ada-112">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="15ada-112">mobileAppIdentifier</span></span>|[<span data-ttu-id="15ada-113">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="15ada-113">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="15ada-114">Bereitstellung einer App</span><span class="sxs-lookup"><span data-stu-id="15ada-114">Deployment of an app.</span></span>|
|<span data-ttu-id="15ada-115">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="15ada-115">configurationAppliedUserCount</span></span>|<span data-ttu-id="15ada-116">Int32</span><span class="sxs-lookup"><span data-stu-id="15ada-116">Int32</span></span>|<span data-ttu-id="15ada-117">Die Anzahl der Benutzer, auf die die Richtlinie angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="15ada-117">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15ada-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="15ada-118">Relationships</span></span>
<span data-ttu-id="15ada-119">Keine</span><span class="sxs-lookup"><span data-stu-id="15ada-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15ada-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="15ada-120">JSON Representation</span></span>
<span data-ttu-id="15ada-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="15ada-121">Here is a JSON representation of the resource.</span></span>
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




