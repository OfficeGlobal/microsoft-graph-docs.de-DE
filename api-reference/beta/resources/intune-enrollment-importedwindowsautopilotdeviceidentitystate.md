---
title: importedWindowsAutopilotDeviceIdentityState-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b8130c354157bcfe679a95914e9266e500a6b51
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972943"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="03317-103">importedWindowsAutopilotDeviceIdentityState-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="03317-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="03317-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="03317-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03317-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="03317-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03317-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="03317-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="03317-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="03317-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="03317-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="03317-108">Properties</span></span>
|<span data-ttu-id="03317-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="03317-109">Property</span></span>|<span data-ttu-id="03317-110">Typ</span><span class="sxs-lookup"><span data-stu-id="03317-110">Type</span></span>|<span data-ttu-id="03317-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="03317-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03317-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="03317-112">deviceImportStatus</span></span>|[<span data-ttu-id="03317-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="03317-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="03317-114">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätestatus.</span><span class="sxs-lookup"><span data-stu-id="03317-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="03317-115">Mögliche Werte: `unknown`, `pending`, `partial`, `complete`, `error`.</span><span class="sxs-lookup"><span data-stu-id="03317-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="03317-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="03317-116">deviceRegistrationId</span></span>|<span data-ttu-id="03317-117">String</span><span class="sxs-lookup"><span data-stu-id="03317-117">String</span></span>|<span data-ttu-id="03317-118">Vom Geräteverzeichnisdienst (DDS) gemeldete Geräteregistrierungs-ID für erfolgreich hinzugefügtes Gerät</span><span class="sxs-lookup"><span data-stu-id="03317-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="03317-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="03317-119">deviceErrorCode</span></span>|<span data-ttu-id="03317-120">Int32</span><span class="sxs-lookup"><span data-stu-id="03317-120">Int32</span></span>|<span data-ttu-id="03317-121">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätefehlercode</span><span class="sxs-lookup"><span data-stu-id="03317-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="03317-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="03317-122">deviceErrorName</span></span>|<span data-ttu-id="03317-123">String</span><span class="sxs-lookup"><span data-stu-id="03317-123">String</span></span>|<span data-ttu-id="03317-124">Vom Geräteverzeichnisdienst (DDS) gemeldeter Gerätefehlername</span><span class="sxs-lookup"><span data-stu-id="03317-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="03317-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="03317-125">Relationships</span></span>
<span data-ttu-id="03317-126">Keine</span><span class="sxs-lookup"><span data-stu-id="03317-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="03317-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="03317-127">JSON Representation</span></span>
<span data-ttu-id="03317-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="03317-128">Here is a JSON representation of the resource.</span></span>
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





