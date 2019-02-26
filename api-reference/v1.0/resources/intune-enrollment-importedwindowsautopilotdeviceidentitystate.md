---
title: importedWindowsAutopilotDeviceIdentityState-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e65de1501bb0480daf195ce910001624cabff98
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261705"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="ea393-103">importedWindowsAutopilotDeviceIdentityState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ea393-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="ea393-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ea393-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea393-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ea393-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ea393-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ea393-106">Properties</span></span>
|<span data-ttu-id="ea393-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ea393-107">Property</span></span>|<span data-ttu-id="ea393-108">Typ</span><span class="sxs-lookup"><span data-stu-id="ea393-108">Type</span></span>|<span data-ttu-id="ea393-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ea393-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea393-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="ea393-110">deviceImportStatus</span></span>|[<span data-ttu-id="ea393-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="ea393-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="ea393-112">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="ea393-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="ea393-113">Mögliche Werte: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="ea393-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="ea393-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="ea393-114">deviceRegistrationId</span></span>|<span data-ttu-id="ea393-115">String</span><span class="sxs-lookup"><span data-stu-id="ea393-115">String</span></span>|<span data-ttu-id="ea393-116">Vom Geräteverzeichnisdienst (DDS) gemeldete Geräteregistrierungs-ID für erfolgreich hinzugefügtes Gerät</span><span class="sxs-lookup"><span data-stu-id="ea393-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="ea393-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="ea393-117">deviceErrorCode</span></span>|<span data-ttu-id="ea393-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ea393-118">Int32</span></span>|<span data-ttu-id="ea393-119">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätefehlercode</span><span class="sxs-lookup"><span data-stu-id="ea393-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="ea393-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="ea393-120">deviceErrorName</span></span>|<span data-ttu-id="ea393-121">String</span><span class="sxs-lookup"><span data-stu-id="ea393-121">String</span></span>|<span data-ttu-id="ea393-122">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätefehlername</span><span class="sxs-lookup"><span data-stu-id="ea393-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea393-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ea393-123">Relationships</span></span>
<span data-ttu-id="ea393-124">Keine</span><span class="sxs-lookup"><span data-stu-id="ea393-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea393-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ea393-125">JSON Representation</span></span>
<span data-ttu-id="ea393-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ea393-126">Here is a JSON representation of the resource.</span></span>
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



