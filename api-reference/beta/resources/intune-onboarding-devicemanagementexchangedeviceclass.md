---
title: deviceManagementExchangeDeviceClass-Ressourcentyp
description: Geräteklasse in Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ffa5f9c9f54722711a2e38116c2f2a3e03a3171e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149567"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="89525-103">deviceManagementExchangeDeviceClass-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="89525-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="89525-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="89525-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89525-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="89525-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89525-106">Geräteklasse in Exchange.</span><span class="sxs-lookup"><span data-stu-id="89525-106">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="89525-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="89525-107">Properties</span></span>
|<span data-ttu-id="89525-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="89525-108">Property</span></span>|<span data-ttu-id="89525-109">Typ</span><span class="sxs-lookup"><span data-stu-id="89525-109">Type</span></span>|<span data-ttu-id="89525-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="89525-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89525-111">name</span><span class="sxs-lookup"><span data-stu-id="89525-111">name</span></span>|<span data-ttu-id="89525-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="89525-112">String</span></span>|<span data-ttu-id="89525-113">Name der Geräteklasse, die von dieser Regel betroffen ist.</span><span class="sxs-lookup"><span data-stu-id="89525-113">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="89525-114">type</span><span class="sxs-lookup"><span data-stu-id="89525-114">type</span></span>|[<span data-ttu-id="89525-115">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="89525-115">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="89525-116">Gerätetyp, der von dieser Regel betroffen ist, beispielsweise Modell, Familie.</span><span class="sxs-lookup"><span data-stu-id="89525-116">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="89525-117">Mögliche Werte: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="89525-117">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89525-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="89525-118">Relationships</span></span>
<span data-ttu-id="89525-119">Keine</span><span class="sxs-lookup"><span data-stu-id="89525-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89525-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="89525-120">JSON Representation</span></span>
<span data-ttu-id="89525-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="89525-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```




