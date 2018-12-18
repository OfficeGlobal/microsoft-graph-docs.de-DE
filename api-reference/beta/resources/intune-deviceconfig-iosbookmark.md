---
title: Ressourcentyp iosBookmark
description: iOS-URL-Textmarke
author: tfitzmac
ms.openlocfilehash: e1577537e57365b2452e956e010f6c3f918bd743
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308400"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="4d128-103">Ressourcentyp iosBookmark</span><span class="sxs-lookup"><span data-stu-id="4d128-103">iosBookmark resource type</span></span>

> <span data-ttu-id="4d128-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4d128-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d128-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d128-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d128-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4d128-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d128-107">iOS-URL-Textmarke</span><span class="sxs-lookup"><span data-stu-id="4d128-107">iOS URL bookmark</span></span>
## <a name="properties"></a><span data-ttu-id="4d128-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4d128-108">Properties</span></span>
|<span data-ttu-id="4d128-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d128-109">Property</span></span>|<span data-ttu-id="4d128-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4d128-110">Type</span></span>|<span data-ttu-id="4d128-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d128-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d128-112">url</span><span class="sxs-lookup"><span data-stu-id="4d128-112">url</span></span>|<span data-ttu-id="4d128-113">String</span><span class="sxs-lookup"><span data-stu-id="4d128-113">String</span></span>|<span data-ttu-id="4d128-114">URL für den Zugriff auf zulässige</span><span class="sxs-lookup"><span data-stu-id="4d128-114">URL allowed to access</span></span>|
|<span data-ttu-id="4d128-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="4d128-115">bookmarkFolder</span></span>|<span data-ttu-id="4d128-116">String</span><span class="sxs-lookup"><span data-stu-id="4d128-116">String</span></span>|<span data-ttu-id="4d128-117">Der Ordner, in dem die Textmarke in Safari hinzugefügt werden soll</span><span class="sxs-lookup"><span data-stu-id="4d128-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="4d128-118">displayName</span><span class="sxs-lookup"><span data-stu-id="4d128-118">displayName</span></span>|<span data-ttu-id="4d128-119">String</span><span class="sxs-lookup"><span data-stu-id="4d128-119">String</span></span>|<span data-ttu-id="4d128-120">Der Anzeigename der Textmarke</span><span class="sxs-lookup"><span data-stu-id="4d128-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d128-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4d128-121">Relationships</span></span>
<span data-ttu-id="4d128-122">Keine</span><span class="sxs-lookup"><span data-stu-id="4d128-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4d128-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4d128-123">JSON Representation</span></span>
<span data-ttu-id="4d128-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4d128-124">Here is a JSON representation of the resource.</span></span>
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





