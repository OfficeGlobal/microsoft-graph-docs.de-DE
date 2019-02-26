---
title: iosBookmark-Ressourcentyp
description: iOS-URL-Lesezeichen
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9de5d95cd14931da850ab9bdaf5c581fd17f09dc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174996"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="54577-103">iosBookmark-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="54577-103">iosBookmark resource type</span></span>

> <span data-ttu-id="54577-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="54577-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54577-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="54577-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54577-106">iOS-URL-Lesezeichen</span><span class="sxs-lookup"><span data-stu-id="54577-106">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="54577-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="54577-107">Properties</span></span>
|<span data-ttu-id="54577-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="54577-108">Property</span></span>|<span data-ttu-id="54577-109">Typ</span><span class="sxs-lookup"><span data-stu-id="54577-109">Type</span></span>|<span data-ttu-id="54577-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="54577-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54577-111">url</span><span class="sxs-lookup"><span data-stu-id="54577-111">url</span></span>|<span data-ttu-id="54577-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54577-112">String</span></span>|<span data-ttu-id="54577-113">URL erlaubt Zugriff</span><span class="sxs-lookup"><span data-stu-id="54577-113">URL allowed to access</span></span>|
|<span data-ttu-id="54577-114">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="54577-114">bookmarkFolder</span></span>|<span data-ttu-id="54577-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="54577-115">String</span></span>|<span data-ttu-id="54577-116">Der Ordner, in dem die Textmarke in Safari hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="54577-116">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="54577-117">displayName</span><span class="sxs-lookup"><span data-stu-id="54577-117">displayName</span></span>|<span data-ttu-id="54577-118">String</span><span class="sxs-lookup"><span data-stu-id="54577-118">String</span></span>|<span data-ttu-id="54577-119">Der Anzeigename der Textmarke</span><span class="sxs-lookup"><span data-stu-id="54577-119">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="54577-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="54577-120">Relationships</span></span>
<span data-ttu-id="54577-121">Keine</span><span class="sxs-lookup"><span data-stu-id="54577-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54577-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="54577-122">JSON Representation</span></span>
<span data-ttu-id="54577-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="54577-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```




