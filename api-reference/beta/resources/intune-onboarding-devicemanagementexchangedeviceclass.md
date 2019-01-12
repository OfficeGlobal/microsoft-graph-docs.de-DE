---
title: Ressourcentyp deviceManagementExchangeDeviceClass
description: Geräteklasse in Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fcc46cf2744563108a7f063faf5fffbfda172394
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986621"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="d4376-103">Ressourcentyp deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="d4376-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="d4376-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d4376-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4376-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4376-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4376-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d4376-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4376-107">Geräteklasse in Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4376-107">Device Class in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="d4376-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4376-108">Properties</span></span>
|<span data-ttu-id="d4376-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4376-109">Property</span></span>|<span data-ttu-id="d4376-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d4376-110">Type</span></span>|<span data-ttu-id="d4376-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4376-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4376-112">name</span><span class="sxs-lookup"><span data-stu-id="d4376-112">name</span></span>|<span data-ttu-id="d4376-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4376-113">String</span></span>|<span data-ttu-id="d4376-114">Name der Geräteklasse die von dieser Regel betroffen sind.</span><span class="sxs-lookup"><span data-stu-id="d4376-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="d4376-115">type</span><span class="sxs-lookup"><span data-stu-id="d4376-115">type</span></span>|[<span data-ttu-id="d4376-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="d4376-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="d4376-117">Typ des Geräts, die durch diese Regel beeinflusst wird, z. B. Modell, Familie.</span><span class="sxs-lookup"><span data-stu-id="d4376-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="d4376-118">Mögliche Werte: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="d4376-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4376-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d4376-119">Relationships</span></span>
<span data-ttu-id="d4376-120">Keine</span><span class="sxs-lookup"><span data-stu-id="d4376-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d4376-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4376-121">JSON Representation</span></span>
<span data-ttu-id="d4376-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d4376-122">Here is a JSON representation of the resource.</span></span>
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





