---
title: Ressourcentyp win32LobAppRegistryDetection
description: Enthält Registrierungseigenschaften zum Erkennen von einer App Win32
author: tfitzmac
ms.openlocfilehash: 5adeca1b569531d15657acc2a8960bab60580dc6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347740"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="a8baf-103">Ressourcentyp win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="a8baf-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="a8baf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a8baf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8baf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8baf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8baf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a8baf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8baf-107">Enthält Registrierungseigenschaften zum Erkennen von einer App Win32</span><span class="sxs-lookup"><span data-stu-id="a8baf-107">Contains registry properties to detect a Win32 App</span></span>

<span data-ttu-id="a8baf-108">Erbt vom [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="a8baf-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a8baf-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a8baf-109">Properties</span></span>
|<span data-ttu-id="a8baf-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8baf-110">Property</span></span>|<span data-ttu-id="a8baf-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a8baf-111">Type</span></span>|<span data-ttu-id="a8baf-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8baf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8baf-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="a8baf-113">check32BitOn64System</span></span>|<span data-ttu-id="a8baf-114">Boolesch</span><span class="sxs-lookup"><span data-stu-id="a8baf-114">Boolean</span></span>|<span data-ttu-id="a8baf-115">Ein Wert, der angibt, ob in diesem Registrierungspfad ist für die Überprüfung auf 32-Bit-app auf 64-Bit-system</span><span class="sxs-lookup"><span data-stu-id="a8baf-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="a8baf-116">keyPath</span><span class="sxs-lookup"><span data-stu-id="a8baf-116">keyPath</span></span>|<span data-ttu-id="a8baf-117">String</span><span class="sxs-lookup"><span data-stu-id="a8baf-117">String</span></span>|<span data-ttu-id="a8baf-118">Registrierungsschlüsselpfad zum Erkennen von Win32 Line of Business (LoB)-app</span><span class="sxs-lookup"><span data-stu-id="a8baf-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="a8baf-119">Wertname</span><span class="sxs-lookup"><span data-stu-id="a8baf-119">valueName</span></span>|<span data-ttu-id="a8baf-120">String</span><span class="sxs-lookup"><span data-stu-id="a8baf-120">String</span></span>|<span data-ttu-id="a8baf-121">Der Name des Registrierungsschlüssels</span><span class="sxs-lookup"><span data-stu-id="a8baf-121">The registry value name</span></span>|
|<span data-ttu-id="a8baf-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="a8baf-122">detectionType</span></span>|[<span data-ttu-id="a8baf-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="a8baf-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="a8baf-124">Der Erkennung Datentyp.</span><span class="sxs-lookup"><span data-stu-id="a8baf-124">The registry data detection type.</span></span> <span data-ttu-id="a8baf-125">Mögliche Werte sind: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer` und `version`.</span><span class="sxs-lookup"><span data-stu-id="a8baf-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="a8baf-126">operator</span><span class="sxs-lookup"><span data-stu-id="a8baf-126">operator</span></span>|[<span data-ttu-id="a8baf-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="a8baf-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="a8baf-128">Der Operator für die Registrierung Daten Erkennung.</span><span class="sxs-lookup"><span data-stu-id="a8baf-128">The operator for registry data detection.</span></span> <span data-ttu-id="a8baf-129">Mögliche Werte sind: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan` und `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="a8baf-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="a8baf-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="a8baf-130">detectionValue</span></span>|<span data-ttu-id="a8baf-131">String</span><span class="sxs-lookup"><span data-stu-id="a8baf-131">String</span></span>|<span data-ttu-id="a8baf-132">Den Registrierungswert Erkennung</span><span class="sxs-lookup"><span data-stu-id="a8baf-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8baf-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a8baf-133">Relationships</span></span>
<span data-ttu-id="a8baf-134">Keine</span><span class="sxs-lookup"><span data-stu-id="a8baf-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8baf-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a8baf-135">JSON Representation</span></span>
<span data-ttu-id="a8baf-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a8baf-136">Here is a JSON representation of the resource.</span></span>
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





