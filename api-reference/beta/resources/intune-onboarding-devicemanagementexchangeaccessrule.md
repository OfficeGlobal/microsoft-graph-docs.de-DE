---
title: Ressourcentyp deviceManagementExchangeAccessRule
description: Gerätezugriffsregeln in Exchange.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c46bff30bf5f88723a789bb13160bf5aedb1ef2a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409440"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="95775-103">Ressourcentyp deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="95775-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="95775-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="95775-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="95775-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="95775-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95775-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="95775-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95775-107">Gerätezugriffsregeln in Exchange.</span><span class="sxs-lookup"><span data-stu-id="95775-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="95775-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="95775-108">Properties</span></span>
|<span data-ttu-id="95775-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="95775-109">Property</span></span>|<span data-ttu-id="95775-110">Typ</span><span class="sxs-lookup"><span data-stu-id="95775-110">Type</span></span>|<span data-ttu-id="95775-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95775-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95775-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="95775-112">deviceClass</span></span>|[<span data-ttu-id="95775-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="95775-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="95775-114">Geräteklasse, die von dieser Regel betroffen sind.</span><span class="sxs-lookup"><span data-stu-id="95775-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="95775-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="95775-115">accessLevel</span></span>|[<span data-ttu-id="95775-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="95775-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="95775-117">Die Zugriffsebene für Exchange durch diese Regel erteilt.</span><span class="sxs-lookup"><span data-stu-id="95775-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="95775-118">Mögliche Werte: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="95775-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95775-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="95775-119">Relationships</span></span>
<span data-ttu-id="95775-120">Keine</span><span class="sxs-lookup"><span data-stu-id="95775-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95775-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="95775-121">JSON Representation</span></span>
<span data-ttu-id="95775-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="95775-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeAccessRule",
  "deviceClass": {
    "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
    "name": "String",
    "type": "String"
  },
  "accessLevel": "String"
}
```




