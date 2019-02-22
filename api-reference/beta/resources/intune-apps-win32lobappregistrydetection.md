---
title: win32LobAppRegistryDetection-Ressourcentyp
description: Enthält Registrierungseigenschaften zum Auffinden einer Win32-App
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 076251ea185359127c3dad3610ec944f7cdb3178
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169545"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="48872-103">win32LobAppRegistryDetection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="48872-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="48872-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="48872-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48872-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="48872-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48872-106">Enthält Registrierungseigenschaften zum Auffinden einer Win32-App</span><span class="sxs-lookup"><span data-stu-id="48872-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="48872-107">Erbt von [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="48872-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="48872-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="48872-108">Properties</span></span>
|<span data-ttu-id="48872-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="48872-109">Property</span></span>|<span data-ttu-id="48872-110">Typ</span><span class="sxs-lookup"><span data-stu-id="48872-110">Type</span></span>|<span data-ttu-id="48872-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48872-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48872-112">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="48872-112">check32BitOn64System</span></span>|<span data-ttu-id="48872-113">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="48872-113">Boolean</span></span>|<span data-ttu-id="48872-114">Ein Wert, der angibt, ob dieser Registrierungspfad zum Überprüfen der 32-Bit-App auf dem 64-Bit-System dient.</span><span class="sxs-lookup"><span data-stu-id="48872-114">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="48872-115">keyPath</span><span class="sxs-lookup"><span data-stu-id="48872-115">keyPath</span></span>|<span data-ttu-id="48872-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48872-116">String</span></span>|<span data-ttu-id="48872-117">Registrierungsschlüsselpfad zum Aufspüren der Win32-Branchen-App</span><span class="sxs-lookup"><span data-stu-id="48872-117">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="48872-118">valueName</span><span class="sxs-lookup"><span data-stu-id="48872-118">valueName</span></span>|<span data-ttu-id="48872-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48872-119">String</span></span>|<span data-ttu-id="48872-120">Der Name des Registrierungswerts</span><span class="sxs-lookup"><span data-stu-id="48872-120">The registry value name</span></span>|
|<span data-ttu-id="48872-121">detectiontype</span><span class="sxs-lookup"><span data-stu-id="48872-121">detectionType</span></span>|[<span data-ttu-id="48872-122">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="48872-122">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="48872-123">Der Erkennungstyp der Registrierungsdaten.</span><span class="sxs-lookup"><span data-stu-id="48872-123">The registry data detection type.</span></span> <span data-ttu-id="48872-124">Mögliche Werte sind: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer` und `version`.</span><span class="sxs-lookup"><span data-stu-id="48872-124">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="48872-125">operator</span><span class="sxs-lookup"><span data-stu-id="48872-125">operator</span></span>|[<span data-ttu-id="48872-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="48872-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="48872-127">Der Operator für die Erkennung von Registrierungsdaten.</span><span class="sxs-lookup"><span data-stu-id="48872-127">The operator for registry data detection.</span></span> <span data-ttu-id="48872-128">Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="48872-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="48872-129">Erkennungs-Value</span><span class="sxs-lookup"><span data-stu-id="48872-129">detectionValue</span></span>|<span data-ttu-id="48872-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48872-130">String</span></span>|<span data-ttu-id="48872-131">Der Registrierungs Erkennungswert</span><span class="sxs-lookup"><span data-stu-id="48872-131">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="48872-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="48872-132">Relationships</span></span>
<span data-ttu-id="48872-133">Keine</span><span class="sxs-lookup"><span data-stu-id="48872-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48872-134">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="48872-134">JSON Representation</span></span>
<span data-ttu-id="48872-135">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="48872-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryDetection",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```




