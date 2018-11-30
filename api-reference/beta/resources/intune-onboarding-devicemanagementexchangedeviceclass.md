---
title: Ressourcentyp deviceManagementExchangeDeviceClass
description: Geräteklasse in Exchange.
ms.openlocfilehash: 53234a97ffd2581eea1a4c480161ec9243a710d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064896"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="b644a-103">Ressourcentyp deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="b644a-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="b644a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b644a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b644a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b644a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b644a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b644a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b644a-107">Geräteklasse in Exchange.</span><span class="sxs-lookup"><span data-stu-id="b644a-107">Device Class in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="b644a-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b644a-108">Properties</span></span>
|<span data-ttu-id="b644a-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b644a-109">Property</span></span>|<span data-ttu-id="b644a-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b644a-110">Type</span></span>|<span data-ttu-id="b644a-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b644a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b644a-112">name</span><span class="sxs-lookup"><span data-stu-id="b644a-112">name</span></span>|<span data-ttu-id="b644a-113">String</span><span class="sxs-lookup"><span data-stu-id="b644a-113">String</span></span>|<span data-ttu-id="b644a-114">Name der Geräteklasse die von dieser Regel betroffen sind.</span><span class="sxs-lookup"><span data-stu-id="b644a-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="b644a-115">Typ</span><span class="sxs-lookup"><span data-stu-id="b644a-115">type</span></span>|[<span data-ttu-id="b644a-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="b644a-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="b644a-117">Typ des Geräts, die durch diese Regel beeinflusst wird, z. B. Modell, Familie.</span><span class="sxs-lookup"><span data-stu-id="b644a-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="b644a-118">Mögliche Werte: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="b644a-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b644a-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b644a-119">Relationships</span></span>
<span data-ttu-id="b644a-120">Keine</span><span class="sxs-lookup"><span data-stu-id="b644a-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b644a-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b644a-121">JSON Representation</span></span>
<span data-ttu-id="b644a-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b644a-122">Here is a JSON representation of the resource.</span></span>
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





