---
title: win32LobAppReturnCode-Ressourcentyp
description: Enthält Rückgabecode Eigenschaften für eine Win32-App
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4402464bd4618f1e33b9b766be529cbe592165c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174587"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="6638e-103">win32LobAppReturnCode-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6638e-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="6638e-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6638e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6638e-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6638e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6638e-106">Enthält Rückgabecode Eigenschaften für eine Win32-App</span><span class="sxs-lookup"><span data-stu-id="6638e-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="6638e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6638e-107">Properties</span></span>
|<span data-ttu-id="6638e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6638e-108">Property</span></span>|<span data-ttu-id="6638e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="6638e-109">Type</span></span>|<span data-ttu-id="6638e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6638e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6638e-111">returnCode</span><span class="sxs-lookup"><span data-stu-id="6638e-111">returnCode</span></span>|<span data-ttu-id="6638e-112">Int32</span><span class="sxs-lookup"><span data-stu-id="6638e-112">Int32</span></span>|<span data-ttu-id="6638e-113">Rückgabecode.</span><span class="sxs-lookup"><span data-stu-id="6638e-113">Return code.</span></span>|
|<span data-ttu-id="6638e-114">type</span><span class="sxs-lookup"><span data-stu-id="6638e-114">type</span></span>|[<span data-ttu-id="6638e-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="6638e-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="6638e-116">Der Typ des Rückgabecodes.</span><span class="sxs-lookup"><span data-stu-id="6638e-116">The type of return code.</span></span> <span data-ttu-id="6638e-117">Mögliche Werte: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span><span class="sxs-lookup"><span data-stu-id="6638e-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6638e-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6638e-118">Relationships</span></span>
<span data-ttu-id="6638e-119">Keine</span><span class="sxs-lookup"><span data-stu-id="6638e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6638e-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6638e-120">JSON Representation</span></span>
<span data-ttu-id="6638e-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6638e-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```




