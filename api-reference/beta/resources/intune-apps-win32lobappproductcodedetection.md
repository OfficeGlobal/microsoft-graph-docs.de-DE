---
title: Ressourcentyp win32LobAppProductCodeDetection
description: Enthält die Eigenschaften Code und Version Produkt, um zu ermitteln, eine Win32-App
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5536384178ac197d3b52609cb767fef82befd3b2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928527"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="5654b-103">Ressourcentyp win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="5654b-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="5654b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5654b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5654b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5654b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5654b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5654b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5654b-107">Enthält die Eigenschaften Code und Version Produkt, um zu ermitteln, eine Win32-App</span><span class="sxs-lookup"><span data-stu-id="5654b-107">Contains product code and version properties to detect a Win32 App</span></span>

<span data-ttu-id="5654b-108">Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="5654b-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5654b-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5654b-109">Properties</span></span>
|<span data-ttu-id="5654b-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5654b-110">Property</span></span>|<span data-ttu-id="5654b-111">Typ</span><span class="sxs-lookup"><span data-stu-id="5654b-111">Type</span></span>|<span data-ttu-id="5654b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5654b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5654b-113">productCode</span><span class="sxs-lookup"><span data-stu-id="5654b-113">productCode</span></span>|<span data-ttu-id="5654b-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5654b-114">String</span></span>|<span data-ttu-id="5654b-115">Den Produktcode Win32 Line of Business (LoB) App.</span><span class="sxs-lookup"><span data-stu-id="5654b-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5654b-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="5654b-116">productVersionOperator</span></span>|[<span data-ttu-id="5654b-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="5654b-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="5654b-118">Der Operator zum Erkennen von Version des Produkts.</span><span class="sxs-lookup"><span data-stu-id="5654b-118">The operator to detect product version.</span></span> <span data-ttu-id="5654b-119">Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="5654b-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="5654b-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="5654b-120">productVersion</span></span>|<span data-ttu-id="5654b-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5654b-121">String</span></span>|<span data-ttu-id="5654b-122">Die Produktversion von Win32 Line of Business (LoB) app.</span><span class="sxs-lookup"><span data-stu-id="5654b-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5654b-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5654b-123">Relationships</span></span>
<span data-ttu-id="5654b-124">Keine</span><span class="sxs-lookup"><span data-stu-id="5654b-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5654b-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5654b-125">JSON Representation</span></span>
<span data-ttu-id="5654b-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5654b-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeDetection",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```





