---
title: Ressourcentyp win32LobAppRegistryDetection
description: Enthält Registrierungseigenschaften zum Erkennen von einer App Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb10a96a14d3c26503b33191fbb3c1b883245da7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402664"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="6a4a1-103">Ressourcentyp win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="6a4a1-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="6a4a1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6a4a1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6a4a1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a4a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a4a1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a4a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a4a1-107">Enthält Registrierungseigenschaften zum Erkennen von einer App Win32</span><span class="sxs-lookup"><span data-stu-id="6a4a1-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="6a4a1-108">Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="6a4a1-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6a4a1-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6a4a1-109">Properties</span></span>
|<span data-ttu-id="6a4a1-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a4a1-110">Property</span></span>|<span data-ttu-id="6a4a1-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6a4a1-111">Type</span></span>|<span data-ttu-id="6a4a1-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a4a1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a4a1-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="6a4a1-113">check32BitOn64System</span></span>|<span data-ttu-id="6a4a1-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a4a1-114">Boolean</span></span>|<span data-ttu-id="6a4a1-115">Ein Wert, der angibt, ob in diesem Registrierungspfad ist für die Überprüfung auf 32-Bit-app auf 64-Bit-system</span><span class="sxs-lookup"><span data-stu-id="6a4a1-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="6a4a1-116">keyPath</span><span class="sxs-lookup"><span data-stu-id="6a4a1-116">keyPath</span></span>|<span data-ttu-id="6a4a1-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a4a1-117">String</span></span>|<span data-ttu-id="6a4a1-118">Registrierungsschlüsselpfad zum Erkennen von Win32 Line of Business (LoB)-app</span><span class="sxs-lookup"><span data-stu-id="6a4a1-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="6a4a1-119">Wertname</span><span class="sxs-lookup"><span data-stu-id="6a4a1-119">valueName</span></span>|<span data-ttu-id="6a4a1-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a4a1-120">String</span></span>|<span data-ttu-id="6a4a1-121">Der Name des Registrierungsschlüssels</span><span class="sxs-lookup"><span data-stu-id="6a4a1-121">The registry value name</span></span>|
|<span data-ttu-id="6a4a1-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="6a4a1-122">detectionType</span></span>|[<span data-ttu-id="6a4a1-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="6a4a1-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="6a4a1-124">Der Erkennung Datentyp.</span><span class="sxs-lookup"><span data-stu-id="6a4a1-124">The registry data detection type.</span></span> <span data-ttu-id="6a4a1-125">Mögliche Werte sind: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer` und `version`.</span><span class="sxs-lookup"><span data-stu-id="6a4a1-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="6a4a1-126">operator</span><span class="sxs-lookup"><span data-stu-id="6a4a1-126">operator</span></span>|[<span data-ttu-id="6a4a1-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="6a4a1-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="6a4a1-128">Der Operator für die Registrierung Daten Erkennung.</span><span class="sxs-lookup"><span data-stu-id="6a4a1-128">The operator for registry data detection.</span></span> <span data-ttu-id="6a4a1-129">Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="6a4a1-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="6a4a1-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="6a4a1-130">detectionValue</span></span>|<span data-ttu-id="6a4a1-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6a4a1-131">String</span></span>|<span data-ttu-id="6a4a1-132">Den Registrierungswert Erkennung</span><span class="sxs-lookup"><span data-stu-id="6a4a1-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a4a1-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6a4a1-133">Relationships</span></span>
<span data-ttu-id="6a4a1-134">Keine</span><span class="sxs-lookup"><span data-stu-id="6a4a1-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a4a1-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6a4a1-135">JSON Representation</span></span>
<span data-ttu-id="6a4a1-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6a4a1-136">Here is a JSON representation of the resource.</span></span>
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




