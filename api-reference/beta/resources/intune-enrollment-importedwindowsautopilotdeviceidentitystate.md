---
title: importedWindowsAutopilotDeviceIdentityState-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72ed544a7b4f9e4ddf003104b191ee064b884f76
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159010"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="20df7-103">importedWindowsAutopilotDeviceIdentityState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="20df7-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="20df7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="20df7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20df7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="20df7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20df7-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="20df7-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="20df7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="20df7-107">Properties</span></span>
|<span data-ttu-id="20df7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="20df7-108">Property</span></span>|<span data-ttu-id="20df7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="20df7-109">Type</span></span>|<span data-ttu-id="20df7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="20df7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20df7-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="20df7-111">deviceImportStatus</span></span>|[<span data-ttu-id="20df7-112">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="20df7-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="20df7-113">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="20df7-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="20df7-114">Mögliche Werte: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="20df7-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="20df7-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="20df7-115">deviceRegistrationId</span></span>|<span data-ttu-id="20df7-116">String</span><span class="sxs-lookup"><span data-stu-id="20df7-116">String</span></span>|<span data-ttu-id="20df7-117">Vom Geräteverzeichnisdienst (DDS) gemeldete Geräteregistrierungs-ID für erfolgreich hinzugefügtes Gerät</span><span class="sxs-lookup"><span data-stu-id="20df7-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="20df7-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="20df7-118">deviceErrorCode</span></span>|<span data-ttu-id="20df7-119">Int32</span><span class="sxs-lookup"><span data-stu-id="20df7-119">Int32</span></span>|<span data-ttu-id="20df7-120">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätefehlercode</span><span class="sxs-lookup"><span data-stu-id="20df7-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="20df7-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="20df7-121">deviceErrorName</span></span>|<span data-ttu-id="20df7-122">String</span><span class="sxs-lookup"><span data-stu-id="20df7-122">String</span></span>|<span data-ttu-id="20df7-123">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätefehlername</span><span class="sxs-lookup"><span data-stu-id="20df7-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="20df7-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="20df7-124">Relationships</span></span>
<span data-ttu-id="20df7-125">Keine</span><span class="sxs-lookup"><span data-stu-id="20df7-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20df7-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="20df7-126">JSON Representation</span></span>
<span data-ttu-id="20df7-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="20df7-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```




