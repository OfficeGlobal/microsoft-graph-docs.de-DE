---
title: win32LobAppProductCodeDetection-Ressourcentyp
description: Enthält Produktcode-und Versionseigenschaften zum Auffinden einer Win32-App
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 854d54b034b0e2e0dc0e7ce8e7f73466f37dd263
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173234"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="88dbe-103">win32LobAppProductCodeDetection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="88dbe-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="88dbe-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="88dbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88dbe-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="88dbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88dbe-106">Enthält Produktcode-und Versionseigenschaften zum Auffinden einer Win32-App</span><span class="sxs-lookup"><span data-stu-id="88dbe-106">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="88dbe-107">Erbt von [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="88dbe-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="88dbe-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="88dbe-108">Properties</span></span>
|<span data-ttu-id="88dbe-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="88dbe-109">Property</span></span>|<span data-ttu-id="88dbe-110">Typ</span><span class="sxs-lookup"><span data-stu-id="88dbe-110">Type</span></span>|<span data-ttu-id="88dbe-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="88dbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88dbe-112">productCode</span><span class="sxs-lookup"><span data-stu-id="88dbe-112">productCode</span></span>|<span data-ttu-id="88dbe-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88dbe-113">String</span></span>|<span data-ttu-id="88dbe-114">Der Produktcode der Win32-Branchen-app.</span><span class="sxs-lookup"><span data-stu-id="88dbe-114">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="88dbe-115">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="88dbe-115">productVersionOperator</span></span>|[<span data-ttu-id="88dbe-116">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="88dbe-116">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="88dbe-117">Der Operator, der die Produktversion ermittelt.</span><span class="sxs-lookup"><span data-stu-id="88dbe-117">The operator to detect product version.</span></span> <span data-ttu-id="88dbe-118">Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="88dbe-118">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="88dbe-119">productVersion</span><span class="sxs-lookup"><span data-stu-id="88dbe-119">productVersion</span></span>|<span data-ttu-id="88dbe-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="88dbe-120">String</span></span>|<span data-ttu-id="88dbe-121">Die Produktversion der Win32-Branchen-app.</span><span class="sxs-lookup"><span data-stu-id="88dbe-121">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88dbe-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="88dbe-122">Relationships</span></span>
<span data-ttu-id="88dbe-123">Keine</span><span class="sxs-lookup"><span data-stu-id="88dbe-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88dbe-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="88dbe-124">JSON Representation</span></span>
<span data-ttu-id="88dbe-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="88dbe-125">Here is a JSON representation of the resource.</span></span>
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




