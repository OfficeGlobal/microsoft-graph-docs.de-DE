---
title: Ressourcentyp unsupportedDeviceConfigurationDetail
description: Eine Beschreibung des warum ein Entity-Objekt nicht unterstützt wird.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c03bdb20fc4c48fa7820e09b9212bf73250599aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400389"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="b54bf-103">Ressourcentyp unsupportedDeviceConfigurationDetail</span><span class="sxs-lookup"><span data-stu-id="b54bf-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="b54bf-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b54bf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b54bf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b54bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b54bf-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b54bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b54bf-107">Eine Beschreibung des warum ein Entity-Objekt nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="b54bf-107">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="b54bf-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b54bf-108">Properties</span></span>
|<span data-ttu-id="b54bf-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b54bf-109">Property</span></span>|<span data-ttu-id="b54bf-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b54bf-110">Type</span></span>|<span data-ttu-id="b54bf-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b54bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b54bf-112">message</span><span class="sxs-lookup"><span data-stu-id="b54bf-112">message</span></span>|<span data-ttu-id="b54bf-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b54bf-113">String</span></span>|<span data-ttu-id="b54bf-114">Eine Nachricht erläutert, warum ein Entity-Objekt nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="b54bf-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="b54bf-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="b54bf-115">propertyName</span></span>|<span data-ttu-id="b54bf-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b54bf-116">String</span></span>|<span data-ttu-id="b54bf-117">Wenn die Nachricht an eine bestimmte Eigenschaft in der ursprünglichen Entität, und klicken Sie dann auf den Namen dieser Eigenschaft verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="b54bf-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b54bf-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b54bf-118">Relationships</span></span>
<span data-ttu-id="b54bf-119">Keine</span><span class="sxs-lookup"><span data-stu-id="b54bf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b54bf-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b54bf-120">JSON Representation</span></span>
<span data-ttu-id="b54bf-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b54bf-121">Here is a JSON representation of the resource.</span></span>
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




