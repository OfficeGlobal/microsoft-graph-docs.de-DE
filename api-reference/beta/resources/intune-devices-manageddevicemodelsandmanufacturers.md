---
title: Ressourcentyp managedDeviceModelsAndManufacturers
description: Modelle und Hersteller Meatadata für verwaltete Geräte im Konto
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a1769f82153fd8184807877c484a4dc31ebda1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927527"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="98ac2-103">Ressourcentyp managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="98ac2-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="98ac2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="98ac2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98ac2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="98ac2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98ac2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="98ac2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98ac2-107">Modelle und Hersteller Meatadata für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="98ac2-107">Models and Manufactures meatadata for managed devices in the account</span></span>
## <a name="properties"></a><span data-ttu-id="98ac2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="98ac2-108">Properties</span></span>
|<span data-ttu-id="98ac2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="98ac2-109">Property</span></span>|<span data-ttu-id="98ac2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="98ac2-110">Type</span></span>|<span data-ttu-id="98ac2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98ac2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98ac2-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="98ac2-112">deviceModels</span></span>|<span data-ttu-id="98ac2-113">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="98ac2-113">String collection</span></span>|<span data-ttu-id="98ac2-114">Liste der Modelle für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="98ac2-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="98ac2-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="98ac2-115">deviceManufacturers</span></span>|<span data-ttu-id="98ac2-116">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="98ac2-116">String collection</span></span>|<span data-ttu-id="98ac2-117">Liste der Hersteller für verwalteten Geräten im Konto</span><span class="sxs-lookup"><span data-stu-id="98ac2-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="98ac2-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="98ac2-118">Relationships</span></span>
<span data-ttu-id="98ac2-119">Keine</span><span class="sxs-lookup"><span data-stu-id="98ac2-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98ac2-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="98ac2-120">JSON Representation</span></span>
<span data-ttu-id="98ac2-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="98ac2-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```





