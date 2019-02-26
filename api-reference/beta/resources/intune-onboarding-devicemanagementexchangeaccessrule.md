---
title: deviceManagementExchangeAccessRule-Ressourcentyp
description: Gerätezugriffsregeln in Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 38b021bc2f0a4ffa19ca551c2621b08f21e8a35e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165779"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="f0512-103">deviceManagementExchangeAccessRule-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f0512-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="f0512-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f0512-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0512-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f0512-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0512-106">Gerätezugriffsregeln in Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0512-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="f0512-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f0512-107">Properties</span></span>
|<span data-ttu-id="f0512-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f0512-108">Property</span></span>|<span data-ttu-id="f0512-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f0512-109">Type</span></span>|<span data-ttu-id="f0512-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f0512-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0512-111">deviceClass</span><span class="sxs-lookup"><span data-stu-id="f0512-111">deviceClass</span></span>|[<span data-ttu-id="f0512-112">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="f0512-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="f0512-113">Geräteklasse, die von dieser Regel betroffen ist.</span><span class="sxs-lookup"><span data-stu-id="f0512-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="f0512-114">Access Level</span><span class="sxs-lookup"><span data-stu-id="f0512-114">accessLevel</span></span>|[<span data-ttu-id="f0512-115">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="f0512-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="f0512-116">Zugriffsebene für Exchange, die von dieser Regel erteilt wird.</span><span class="sxs-lookup"><span data-stu-id="f0512-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="f0512-117">Mögliche Werte: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="f0512-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0512-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f0512-118">Relationships</span></span>
<span data-ttu-id="f0512-119">Keine</span><span class="sxs-lookup"><span data-stu-id="f0512-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0512-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f0512-120">JSON Representation</span></span>
<span data-ttu-id="f0512-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f0512-121">Here is a JSON representation of the resource.</span></span>
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




