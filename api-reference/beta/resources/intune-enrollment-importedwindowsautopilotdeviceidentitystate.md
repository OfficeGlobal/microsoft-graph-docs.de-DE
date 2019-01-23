---
title: importedWindowsAutopilotDeviceIdentityState-Ressourcentyp
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0f4e76b23d4d970a9fb873326dc84f278aa2ed2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410966"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="bec64-103">importedWindowsAutopilotDeviceIdentityState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bec64-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="bec64-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="bec64-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bec64-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bec64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bec64-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bec64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bec64-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bec64-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bec64-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bec64-108">Properties</span></span>
|<span data-ttu-id="bec64-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bec64-109">Property</span></span>|<span data-ttu-id="bec64-110">Typ</span><span class="sxs-lookup"><span data-stu-id="bec64-110">Type</span></span>|<span data-ttu-id="bec64-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bec64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bec64-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="bec64-112">deviceImportStatus</span></span>|[<span data-ttu-id="bec64-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="bec64-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="bec64-114">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="bec64-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="bec64-115">Mögliche Werte: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="bec64-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="bec64-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="bec64-116">deviceRegistrationId</span></span>|<span data-ttu-id="bec64-117">String</span><span class="sxs-lookup"><span data-stu-id="bec64-117">String</span></span>|<span data-ttu-id="bec64-118">Vom Geräteverzeichnisdienst (DDS) gemeldete Geräteregistrierungs-ID für erfolgreich hinzugefügtes Gerät</span><span class="sxs-lookup"><span data-stu-id="bec64-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="bec64-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="bec64-119">deviceErrorCode</span></span>|<span data-ttu-id="bec64-120">Int32</span><span class="sxs-lookup"><span data-stu-id="bec64-120">Int32</span></span>|<span data-ttu-id="bec64-121">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätefehlercode</span><span class="sxs-lookup"><span data-stu-id="bec64-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="bec64-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="bec64-122">deviceErrorName</span></span>|<span data-ttu-id="bec64-123">String</span><span class="sxs-lookup"><span data-stu-id="bec64-123">String</span></span>|<span data-ttu-id="bec64-124">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätefehlername</span><span class="sxs-lookup"><span data-stu-id="bec64-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="bec64-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bec64-125">Relationships</span></span>
<span data-ttu-id="bec64-126">Keine</span><span class="sxs-lookup"><span data-stu-id="bec64-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bec64-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bec64-127">JSON Representation</span></span>
<span data-ttu-id="bec64-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bec64-128">Here is a JSON representation of the resource.</span></span>
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




