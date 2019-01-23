---
title: Ressourcentyp deviceManagementExchangeDeviceClass
description: Geräteklasse in Exchange.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e512253a9b9bc4228d41c369501bec1e7a5e031
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413731"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="c14b2-103">Ressourcentyp deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="c14b2-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="c14b2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c14b2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c14b2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c14b2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c14b2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c14b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c14b2-107">Geräteklasse in Exchange.</span><span class="sxs-lookup"><span data-stu-id="c14b2-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="c14b2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c14b2-108">Properties</span></span>
|<span data-ttu-id="c14b2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c14b2-109">Property</span></span>|<span data-ttu-id="c14b2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c14b2-110">Type</span></span>|<span data-ttu-id="c14b2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c14b2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c14b2-112">name</span><span class="sxs-lookup"><span data-stu-id="c14b2-112">name</span></span>|<span data-ttu-id="c14b2-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c14b2-113">String</span></span>|<span data-ttu-id="c14b2-114">Name der Geräteklasse die von dieser Regel betroffen sind.</span><span class="sxs-lookup"><span data-stu-id="c14b2-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="c14b2-115">type</span><span class="sxs-lookup"><span data-stu-id="c14b2-115">type</span></span>|[<span data-ttu-id="c14b2-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="c14b2-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="c14b2-117">Typ des Geräts, die durch diese Regel beeinflusst wird, z. B. Modell, Familie.</span><span class="sxs-lookup"><span data-stu-id="c14b2-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="c14b2-118">Mögliche Werte: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="c14b2-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c14b2-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c14b2-119">Relationships</span></span>
<span data-ttu-id="c14b2-120">Keine</span><span class="sxs-lookup"><span data-stu-id="c14b2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c14b2-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c14b2-121">JSON Representation</span></span>
<span data-ttu-id="c14b2-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c14b2-122">Here is a JSON representation of the resource.</span></span>
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




