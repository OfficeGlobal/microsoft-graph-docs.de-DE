---
title: Ressourcentyp unsupportedDeviceConfigurationDetail
description: Eine Beschreibung des warum ein Entity-Objekt nicht unterstützt wird.
ms.openlocfilehash: d64d6aedf5da0f3cd79e2582d84fa4f19ea7ccfa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059720"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="a68d5-103">Ressourcentyp unsupportedDeviceConfigurationDetail</span><span class="sxs-lookup"><span data-stu-id="a68d5-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="a68d5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a68d5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a68d5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a68d5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a68d5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a68d5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a68d5-107">Eine Beschreibung des warum ein Entity-Objekt nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="a68d5-107">A description of why an entity is unsupported.</span></span>
## <a name="properties"></a><span data-ttu-id="a68d5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a68d5-108">Properties</span></span>
|<span data-ttu-id="a68d5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a68d5-109">Property</span></span>|<span data-ttu-id="a68d5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a68d5-110">Type</span></span>|<span data-ttu-id="a68d5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a68d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a68d5-112">message</span><span class="sxs-lookup"><span data-stu-id="a68d5-112">message</span></span>|<span data-ttu-id="a68d5-113">String</span><span class="sxs-lookup"><span data-stu-id="a68d5-113">String</span></span>|<span data-ttu-id="a68d5-114">Eine Nachricht erläutert, warum ein Entity-Objekt nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="a68d5-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="a68d5-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="a68d5-115">propertyName</span></span>|<span data-ttu-id="a68d5-116">String</span><span class="sxs-lookup"><span data-stu-id="a68d5-116">String</span></span>|<span data-ttu-id="a68d5-117">Wenn die Nachricht an eine bestimmte Eigenschaft in der ursprünglichen Entität, und klicken Sie dann auf den Namen dieser Eigenschaft verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="a68d5-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a68d5-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a68d5-118">Relationships</span></span>
<span data-ttu-id="a68d5-119">Keine</span><span class="sxs-lookup"><span data-stu-id="a68d5-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a68d5-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a68d5-120">JSON Representation</span></span>
<span data-ttu-id="a68d5-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a68d5-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```





