---
title: importedWindowsAutopilotDeviceIdentityState-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 35712bbd8bf0f13ace167cbb7d382a9ba23a319f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977430"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="725ca-103">importedWindowsAutopilotDeviceIdentityState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="725ca-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="725ca-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="725ca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="725ca-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="725ca-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="725ca-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="725ca-106">Properties</span></span>
|<span data-ttu-id="725ca-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="725ca-107">Property</span></span>|<span data-ttu-id="725ca-108">Typ</span><span class="sxs-lookup"><span data-stu-id="725ca-108">Type</span></span>|<span data-ttu-id="725ca-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="725ca-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="725ca-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="725ca-110">deviceImportStatus</span></span>|[<span data-ttu-id="725ca-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="725ca-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="725ca-112">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="725ca-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="725ca-113">Mögliche Werte: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="725ca-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="725ca-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="725ca-114">deviceRegistrationId</span></span>|<span data-ttu-id="725ca-115">String</span><span class="sxs-lookup"><span data-stu-id="725ca-115">String</span></span>|<span data-ttu-id="725ca-116">Vom Geräteverzeichnisdienst (DDS) gemeldete Geräteregistrierungs-ID für erfolgreich hinzugefügtes Gerät</span><span class="sxs-lookup"><span data-stu-id="725ca-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="725ca-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="725ca-117">deviceErrorCode</span></span>|<span data-ttu-id="725ca-118">Int32</span><span class="sxs-lookup"><span data-stu-id="725ca-118">Int32</span></span>|<span data-ttu-id="725ca-119">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätefehlercode</span><span class="sxs-lookup"><span data-stu-id="725ca-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="725ca-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="725ca-120">deviceErrorName</span></span>|<span data-ttu-id="725ca-121">String</span><span class="sxs-lookup"><span data-stu-id="725ca-121">String</span></span>|<span data-ttu-id="725ca-122">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätefehlername</span><span class="sxs-lookup"><span data-stu-id="725ca-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="725ca-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="725ca-123">Relationships</span></span>
<span data-ttu-id="725ca-124">Keine</span><span class="sxs-lookup"><span data-stu-id="725ca-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="725ca-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="725ca-125">JSON Representation</span></span>
<span data-ttu-id="725ca-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="725ca-126">Here is a JSON representation of the resource.</span></span>
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



