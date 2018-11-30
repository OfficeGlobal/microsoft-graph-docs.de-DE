---
title: Ressourcentyp managedDeviceModelsAndManufacturers
description: Modelle und Hersteller Meatadata für verwaltete Geräte im Konto
ms.openlocfilehash: c61026a6caa097e01e09a4343dd54f769c743460
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065943"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a><span data-ttu-id="1d521-103">Ressourcentyp managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="1d521-103">managedDeviceModelsAndManufacturers resource type</span></span>

> <span data-ttu-id="1d521-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1d521-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d521-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1d521-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d521-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1d521-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d521-107">Modelle und Hersteller Meatadata für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="1d521-107">Models and Manufactures meatadata for managed devices in the account</span></span>
## <a name="properties"></a><span data-ttu-id="1d521-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="1d521-108">Properties</span></span>
|<span data-ttu-id="1d521-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1d521-109">Property</span></span>|<span data-ttu-id="1d521-110">Typ</span><span class="sxs-lookup"><span data-stu-id="1d521-110">Type</span></span>|<span data-ttu-id="1d521-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1d521-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d521-112">deviceModels</span><span class="sxs-lookup"><span data-stu-id="1d521-112">deviceModels</span></span>|<span data-ttu-id="1d521-113">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="1d521-113">String collection</span></span>|<span data-ttu-id="1d521-114">Liste der Modelle für verwaltete Geräte im Konto</span><span class="sxs-lookup"><span data-stu-id="1d521-114">List of Models for managed devices in the account</span></span>|
|<span data-ttu-id="1d521-115">deviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="1d521-115">deviceManufacturers</span></span>|<span data-ttu-id="1d521-116">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="1d521-116">String collection</span></span>|<span data-ttu-id="1d521-117">Liste der Hersteller für verwalteten Geräten im Konto</span><span class="sxs-lookup"><span data-stu-id="1d521-117">List of Manufactures for managed devices in the account</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d521-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="1d521-118">Relationships</span></span>
<span data-ttu-id="1d521-119">Keine</span><span class="sxs-lookup"><span data-stu-id="1d521-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1d521-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="1d521-120">JSON Representation</span></span>
<span data-ttu-id="1d521-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="1d521-121">Here is a JSON representation of the resource.</span></span>
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





