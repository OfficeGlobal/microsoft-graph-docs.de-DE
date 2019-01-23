---
title: Ressourcentyp win32LobAppProductCodeDetection
description: Enthält die Eigenschaften Code und Version Produkt, um zu ermitteln, eine Win32-App
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f5af1cfc5fffe5241ef3b7883c3ebe6a2100278
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411204"
---
# <a name="win32lobappproductcodedetection-resource-type"></a><span data-ttu-id="4efc6-103">Ressourcentyp win32LobAppProductCodeDetection</span><span class="sxs-lookup"><span data-stu-id="4efc6-103">win32LobAppProductCodeDetection resource type</span></span>

> <span data-ttu-id="4efc6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4efc6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4efc6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4efc6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4efc6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4efc6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4efc6-107">Enthält die Eigenschaften Code und Version Produkt, um zu ermitteln, eine Win32-App</span><span class="sxs-lookup"><span data-stu-id="4efc6-107">Contains product code and version properties to detect a Win32 App</span></span>


<span data-ttu-id="4efc6-108">Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="4efc6-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4efc6-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4efc6-109">Properties</span></span>
|<span data-ttu-id="4efc6-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4efc6-110">Property</span></span>|<span data-ttu-id="4efc6-111">Typ</span><span class="sxs-lookup"><span data-stu-id="4efc6-111">Type</span></span>|<span data-ttu-id="4efc6-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4efc6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4efc6-113">productCode</span><span class="sxs-lookup"><span data-stu-id="4efc6-113">productCode</span></span>|<span data-ttu-id="4efc6-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4efc6-114">String</span></span>|<span data-ttu-id="4efc6-115">Den Produktcode Win32 Line of Business (LoB) App.</span><span class="sxs-lookup"><span data-stu-id="4efc6-115">The product code of Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4efc6-116">productVersionOperator</span><span class="sxs-lookup"><span data-stu-id="4efc6-116">productVersionOperator</span></span>|[<span data-ttu-id="4efc6-117">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="4efc6-117">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="4efc6-118">Der Operator zum Erkennen von Version des Produkts.</span><span class="sxs-lookup"><span data-stu-id="4efc6-118">The operator to detect product version.</span></span> <span data-ttu-id="4efc6-119">Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="4efc6-119">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="4efc6-120">productVersion</span><span class="sxs-lookup"><span data-stu-id="4efc6-120">productVersion</span></span>|<span data-ttu-id="4efc6-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4efc6-121">String</span></span>|<span data-ttu-id="4efc6-122">Die Produktversion von Win32 Line of Business (LoB) app.</span><span class="sxs-lookup"><span data-stu-id="4efc6-122">The product version of Win32 Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4efc6-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4efc6-123">Relationships</span></span>
<span data-ttu-id="4efc6-124">Keine</span><span class="sxs-lookup"><span data-stu-id="4efc6-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4efc6-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4efc6-125">JSON Representation</span></span>
<span data-ttu-id="4efc6-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4efc6-126">Here is a JSON representation of the resource.</span></span>
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




