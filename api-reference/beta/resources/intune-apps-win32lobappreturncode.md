---
title: Ressourcentyp win32LobAppReturnCode
description: Enthält Eigenschaften Rückgabecode für eine Win32-App
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e6357d0ac6aab87e236e02d60454d1b45aa98fe1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404358"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="8ee71-103">Ressourcentyp win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="8ee71-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="8ee71-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8ee71-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8ee71-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ee71-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ee71-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8ee71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ee71-107">Enthält Eigenschaften Rückgabecode für eine Win32-App</span><span class="sxs-lookup"><span data-stu-id="8ee71-107">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="8ee71-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8ee71-108">Properties</span></span>
|<span data-ttu-id="8ee71-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8ee71-109">Property</span></span>|<span data-ttu-id="8ee71-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8ee71-110">Type</span></span>|<span data-ttu-id="8ee71-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ee71-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ee71-112">Rückgabecode</span><span class="sxs-lookup"><span data-stu-id="8ee71-112">returnCode</span></span>|<span data-ttu-id="8ee71-113">Int32</span><span class="sxs-lookup"><span data-stu-id="8ee71-113">Int32</span></span>|<span data-ttu-id="8ee71-114">Rückgabecode.</span><span class="sxs-lookup"><span data-stu-id="8ee71-114">Return code.</span></span>|
|<span data-ttu-id="8ee71-115">type</span><span class="sxs-lookup"><span data-stu-id="8ee71-115">type</span></span>|[<span data-ttu-id="8ee71-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="8ee71-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="8ee71-117">Der Typ der Rückgabecode.</span><span class="sxs-lookup"><span data-stu-id="8ee71-117">The type of return code.</span></span> <span data-ttu-id="8ee71-118">Mögliche Werte sind: `failed`, `success`, `softReboot`, `hardReboot` und `retry`.</span><span class="sxs-lookup"><span data-stu-id="8ee71-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ee71-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8ee71-119">Relationships</span></span>
<span data-ttu-id="8ee71-120">Keine</span><span class="sxs-lookup"><span data-stu-id="8ee71-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ee71-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8ee71-121">JSON Representation</span></span>
<span data-ttu-id="8ee71-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8ee71-122">Here is a JSON representation of the resource.</span></span>
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




