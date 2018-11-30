---
title: Ressourcentyp deviceManagementExchangeAccessRule
description: Gerätezugriffsregeln in Exchange.
ms.openlocfilehash: e59c81fdfe6cb6a0a7f7f952e6bfc8929bbc2633
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061106"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="b528b-103">Ressourcentyp deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="b528b-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="b528b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b528b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b528b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b528b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b528b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b528b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b528b-107">Gerätezugriffsregeln in Exchange.</span><span class="sxs-lookup"><span data-stu-id="b528b-107">Device Access Rules in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="b528b-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b528b-108">Properties</span></span>
|<span data-ttu-id="b528b-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b528b-109">Property</span></span>|<span data-ttu-id="b528b-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b528b-110">Type</span></span>|<span data-ttu-id="b528b-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b528b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b528b-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="b528b-112">deviceClass</span></span>|[<span data-ttu-id="b528b-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="b528b-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="b528b-114">Geräteklasse, die von dieser Regel betroffen sind.</span><span class="sxs-lookup"><span data-stu-id="b528b-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="b528b-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="b528b-115">accessLevel</span></span>|[<span data-ttu-id="b528b-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="b528b-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="b528b-117">Die Zugriffsebene für Exchange durch diese Regel erteilt.</span><span class="sxs-lookup"><span data-stu-id="b528b-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="b528b-118">Mögliche Werte: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="b528b-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b528b-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b528b-119">Relationships</span></span>
<span data-ttu-id="b528b-120">Keine</span><span class="sxs-lookup"><span data-stu-id="b528b-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b528b-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b528b-121">JSON Representation</span></span>
<span data-ttu-id="b528b-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b528b-122">Here is a JSON representation of the resource.</span></span>
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





