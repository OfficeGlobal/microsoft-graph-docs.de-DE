---
title: Ressourcentyp win32LobAppRegistryDetection
description: Enthält Registrierungseigenschaften zum Erkennen von einer App Win32
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: faccc030a9f15b511af4123c94687c904e60ff10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867137"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="fdb36-103">Ressourcentyp win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="fdb36-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="fdb36-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fdb36-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdb36-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fdb36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdb36-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fdb36-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdb36-107">Enthält Registrierungseigenschaften zum Erkennen von einer App Win32</span><span class="sxs-lookup"><span data-stu-id="fdb36-107">Contains registry properties to detect a Win32 App</span></span>

<span data-ttu-id="fdb36-108">Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="fdb36-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fdb36-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fdb36-109">Properties</span></span>
|<span data-ttu-id="fdb36-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fdb36-110">Property</span></span>|<span data-ttu-id="fdb36-111">Typ</span><span class="sxs-lookup"><span data-stu-id="fdb36-111">Type</span></span>|<span data-ttu-id="fdb36-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdb36-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdb36-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="fdb36-113">check32BitOn64System</span></span>|<span data-ttu-id="fdb36-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="fdb36-114">Boolean</span></span>|<span data-ttu-id="fdb36-115">Ein Wert, der angibt, ob in diesem Registrierungspfad ist für die Überprüfung auf 32-Bit-app auf 64-Bit-system</span><span class="sxs-lookup"><span data-stu-id="fdb36-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="fdb36-116">keyPath</span><span class="sxs-lookup"><span data-stu-id="fdb36-116">keyPath</span></span>|<span data-ttu-id="fdb36-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fdb36-117">String</span></span>|<span data-ttu-id="fdb36-118">Registrierungsschlüsselpfad zum Erkennen von Win32 Line of Business (LoB)-app</span><span class="sxs-lookup"><span data-stu-id="fdb36-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="fdb36-119">Wertname</span><span class="sxs-lookup"><span data-stu-id="fdb36-119">valueName</span></span>|<span data-ttu-id="fdb36-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fdb36-120">String</span></span>|<span data-ttu-id="fdb36-121">Der Name des Registrierungsschlüssels</span><span class="sxs-lookup"><span data-stu-id="fdb36-121">The registry value name</span></span>|
|<span data-ttu-id="fdb36-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="fdb36-122">detectionType</span></span>|[<span data-ttu-id="fdb36-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="fdb36-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="fdb36-124">Der Erkennung Datentyp.</span><span class="sxs-lookup"><span data-stu-id="fdb36-124">The registry data detection type.</span></span> <span data-ttu-id="fdb36-125">Mögliche Werte sind: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer` und `version`.</span><span class="sxs-lookup"><span data-stu-id="fdb36-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="fdb36-126">operator</span><span class="sxs-lookup"><span data-stu-id="fdb36-126">operator</span></span>|[<span data-ttu-id="fdb36-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="fdb36-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="fdb36-128">Der Operator für die Registrierung Daten Erkennung.</span><span class="sxs-lookup"><span data-stu-id="fdb36-128">The operator for registry data detection.</span></span> <span data-ttu-id="fdb36-129">Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="fdb36-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="fdb36-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="fdb36-130">detectionValue</span></span>|<span data-ttu-id="fdb36-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fdb36-131">String</span></span>|<span data-ttu-id="fdb36-132">Den Registrierungswert Erkennung</span><span class="sxs-lookup"><span data-stu-id="fdb36-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdb36-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fdb36-133">Relationships</span></span>
<span data-ttu-id="fdb36-134">Keine</span><span class="sxs-lookup"><span data-stu-id="fdb36-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fdb36-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fdb36-135">JSON Representation</span></span>
<span data-ttu-id="fdb36-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fdb36-136">Here is a JSON representation of the resource.</span></span>
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





