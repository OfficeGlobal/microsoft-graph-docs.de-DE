---
title: Ressourcentyp iosBookmark
description: iOS-URL-Textmarke
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e95f3bfd40bdf5ca5782aa9233a020623d32d6a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395909"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="bc18e-103">Ressourcentyp iosBookmark</span><span class="sxs-lookup"><span data-stu-id="bc18e-103">iosBookmark resource type</span></span>

> <span data-ttu-id="bc18e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="bc18e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc18e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc18e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc18e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc18e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc18e-107">iOS-URL-Textmarke</span><span class="sxs-lookup"><span data-stu-id="bc18e-107">iOS URL bookmark</span></span>

## <a name="properties"></a><span data-ttu-id="bc18e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc18e-108">Properties</span></span>
|<span data-ttu-id="bc18e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc18e-109">Property</span></span>|<span data-ttu-id="bc18e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="bc18e-110">Type</span></span>|<span data-ttu-id="bc18e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc18e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc18e-112">url</span><span class="sxs-lookup"><span data-stu-id="bc18e-112">url</span></span>|<span data-ttu-id="bc18e-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc18e-113">String</span></span>|<span data-ttu-id="bc18e-114">URL für den Zugriff auf zulässige</span><span class="sxs-lookup"><span data-stu-id="bc18e-114">URL allowed to access</span></span>|
|<span data-ttu-id="bc18e-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="bc18e-115">bookmarkFolder</span></span>|<span data-ttu-id="bc18e-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc18e-116">String</span></span>|<span data-ttu-id="bc18e-117">Der Ordner, in dem die Textmarke in Safari hinzugefügt werden soll</span><span class="sxs-lookup"><span data-stu-id="bc18e-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="bc18e-118">displayName</span><span class="sxs-lookup"><span data-stu-id="bc18e-118">displayName</span></span>|<span data-ttu-id="bc18e-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc18e-119">String</span></span>|<span data-ttu-id="bc18e-120">Der Anzeigename der Textmarke</span><span class="sxs-lookup"><span data-stu-id="bc18e-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc18e-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bc18e-121">Relationships</span></span>
<span data-ttu-id="bc18e-122">Keine</span><span class="sxs-lookup"><span data-stu-id="bc18e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc18e-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bc18e-123">JSON Representation</span></span>
<span data-ttu-id="bc18e-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bc18e-124">Here is a JSON representation of the resource.</span></span>
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




