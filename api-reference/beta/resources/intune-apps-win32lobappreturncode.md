---
title: Ressourcentyp win32LobAppReturnCode
description: Enthält Eigenschaften Rückgabecode für eine Win32-App
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f635c49ece6a1083ef3a89271faf76e01206e9ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849819"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="0a059-103">Ressourcentyp win32LobAppReturnCode</span><span class="sxs-lookup"><span data-stu-id="0a059-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="0a059-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0a059-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a059-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a059-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a059-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0a059-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a059-107">Enthält Eigenschaften Rückgabecode für eine Win32-App</span><span class="sxs-lookup"><span data-stu-id="0a059-107">Contains return code properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="0a059-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0a059-108">Properties</span></span>
|<span data-ttu-id="0a059-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a059-109">Property</span></span>|<span data-ttu-id="0a059-110">Typ</span><span class="sxs-lookup"><span data-stu-id="0a059-110">Type</span></span>|<span data-ttu-id="0a059-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a059-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a059-112">Rückgabecode</span><span class="sxs-lookup"><span data-stu-id="0a059-112">returnCode</span></span>|<span data-ttu-id="0a059-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0a059-113">Int32</span></span>|<span data-ttu-id="0a059-114">Rückgabecode.</span><span class="sxs-lookup"><span data-stu-id="0a059-114">Return code.</span></span>|
|<span data-ttu-id="0a059-115">type</span><span class="sxs-lookup"><span data-stu-id="0a059-115">type</span></span>|[<span data-ttu-id="0a059-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="0a059-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="0a059-117">Der Typ der Rückgabecode.</span><span class="sxs-lookup"><span data-stu-id="0a059-117">The type of return code.</span></span> <span data-ttu-id="0a059-118">Mögliche Werte sind: `failed`, `success`, `softReboot`, `hardReboot` und `retry`.</span><span class="sxs-lookup"><span data-stu-id="0a059-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a059-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0a059-119">Relationships</span></span>
<span data-ttu-id="0a059-120">Keine</span><span class="sxs-lookup"><span data-stu-id="0a059-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a059-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0a059-121">JSON Representation</span></span>
<span data-ttu-id="0a059-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0a059-122">Here is a JSON representation of the resource.</span></span>
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





