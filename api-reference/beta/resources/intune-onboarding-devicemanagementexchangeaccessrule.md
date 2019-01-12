---
title: Ressourcentyp deviceManagementExchangeAccessRule
description: Gerätezugriffsregeln in Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a03fb9f56361cc72bd0321a3b2bd548571740b34
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927814"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="6868d-103">Ressourcentyp deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="6868d-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="6868d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6868d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6868d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6868d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6868d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6868d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6868d-107">Gerätezugriffsregeln in Exchange.</span><span class="sxs-lookup"><span data-stu-id="6868d-107">Device Access Rules in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="6868d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6868d-108">Properties</span></span>
|<span data-ttu-id="6868d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6868d-109">Property</span></span>|<span data-ttu-id="6868d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6868d-110">Type</span></span>|<span data-ttu-id="6868d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6868d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6868d-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="6868d-112">deviceClass</span></span>|[<span data-ttu-id="6868d-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="6868d-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="6868d-114">Geräteklasse, die von dieser Regel betroffen sind.</span><span class="sxs-lookup"><span data-stu-id="6868d-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="6868d-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="6868d-115">accessLevel</span></span>|[<span data-ttu-id="6868d-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="6868d-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="6868d-117">Die Zugriffsebene für Exchange durch diese Regel erteilt.</span><span class="sxs-lookup"><span data-stu-id="6868d-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="6868d-118">Mögliche Werte: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="6868d-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6868d-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6868d-119">Relationships</span></span>
<span data-ttu-id="6868d-120">Keine</span><span class="sxs-lookup"><span data-stu-id="6868d-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6868d-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6868d-121">JSON Representation</span></span>
<span data-ttu-id="6868d-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6868d-122">Here is a JSON representation of the resource.</span></span>
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





