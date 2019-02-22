---
title: unsupportedDeviceConfigurationDetail-Ressourcentyp
description: Eine Beschreibung, warum eine Entität nicht unterstützt wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ebdb6eb91dd64c1605288cc0cb1260f8fe7440a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148468"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="d828e-103">unsupportedDeviceConfigurationDetail-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d828e-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="d828e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d828e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d828e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d828e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d828e-106">Eine Beschreibung, warum eine Entität nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="d828e-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="d828e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d828e-107">Properties</span></span>
|<span data-ttu-id="d828e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d828e-108">Property</span></span>|<span data-ttu-id="d828e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d828e-109">Type</span></span>|<span data-ttu-id="d828e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d828e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d828e-111">message</span><span class="sxs-lookup"><span data-stu-id="d828e-111">message</span></span>|<span data-ttu-id="d828e-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d828e-112">String</span></span>|<span data-ttu-id="d828e-113">Eine Meldung, die erklärt, warum eine Entität nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="d828e-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="d828e-114">propertyName</span><span class="sxs-lookup"><span data-stu-id="d828e-114">propertyName</span></span>|<span data-ttu-id="d828e-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d828e-115">String</span></span>|<span data-ttu-id="d828e-116">Wenn die Nachricht mit einer bestimmten Eigenschaft in der ursprünglichen Entität verknüpft ist, dann der Name dieser Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="d828e-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d828e-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d828e-117">Relationships</span></span>
<span data-ttu-id="d828e-118">Keine</span><span class="sxs-lookup"><span data-stu-id="d828e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d828e-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d828e-119">JSON Representation</span></span>
<span data-ttu-id="d828e-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d828e-120">Here is a JSON representation of the resource.</span></span>
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




