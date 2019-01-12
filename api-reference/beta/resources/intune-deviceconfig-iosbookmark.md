---
title: Ressourcentyp iosBookmark
description: iOS-URL-Textmarke
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbf39a2eee5064b7d3ddfa474b1f70758d4c7047
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938174"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="ff383-103">Ressourcentyp iosBookmark</span><span class="sxs-lookup"><span data-stu-id="ff383-103">iosBookmark resource type</span></span>

> <span data-ttu-id="ff383-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff383-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff383-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff383-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff383-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff383-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff383-107">iOS-URL-Textmarke</span><span class="sxs-lookup"><span data-stu-id="ff383-107">iOS URL bookmark</span></span>
## <a name="properties"></a><span data-ttu-id="ff383-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ff383-108">Properties</span></span>
|<span data-ttu-id="ff383-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff383-109">Property</span></span>|<span data-ttu-id="ff383-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ff383-110">Type</span></span>|<span data-ttu-id="ff383-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff383-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff383-112">url</span><span class="sxs-lookup"><span data-stu-id="ff383-112">url</span></span>|<span data-ttu-id="ff383-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff383-113">String</span></span>|<span data-ttu-id="ff383-114">URL für den Zugriff auf zulässige</span><span class="sxs-lookup"><span data-stu-id="ff383-114">URL allowed to access</span></span>|
|<span data-ttu-id="ff383-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="ff383-115">bookmarkFolder</span></span>|<span data-ttu-id="ff383-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff383-116">String</span></span>|<span data-ttu-id="ff383-117">Der Ordner, in dem die Textmarke in Safari hinzugefügt werden soll</span><span class="sxs-lookup"><span data-stu-id="ff383-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="ff383-118">displayName</span><span class="sxs-lookup"><span data-stu-id="ff383-118">displayName</span></span>|<span data-ttu-id="ff383-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ff383-119">String</span></span>|<span data-ttu-id="ff383-120">Der Anzeigename der Textmarke</span><span class="sxs-lookup"><span data-stu-id="ff383-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff383-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ff383-121">Relationships</span></span>
<span data-ttu-id="ff383-122">Keine</span><span class="sxs-lookup"><span data-stu-id="ff383-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff383-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ff383-123">JSON Representation</span></span>
<span data-ttu-id="ff383-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ff383-124">Here is a JSON representation of the resource.</span></span>
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





