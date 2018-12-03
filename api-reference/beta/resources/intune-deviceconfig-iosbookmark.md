---
title: Ressourcentyp iosBookmark
description: iOS-URL-Textmarke
ms.openlocfilehash: e2349e0d280c9798a03363ab90d378ff206c57bf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060419"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="66df9-103">Ressourcentyp iosBookmark</span><span class="sxs-lookup"><span data-stu-id="66df9-103">iosBookmark resource type</span></span>

> <span data-ttu-id="66df9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="66df9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66df9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66df9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66df9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="66df9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66df9-107">iOS-URL-Textmarke</span><span class="sxs-lookup"><span data-stu-id="66df9-107">iOS URL bookmark</span></span>
## <a name="properties"></a><span data-ttu-id="66df9-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66df9-108">Properties</span></span>
|<span data-ttu-id="66df9-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66df9-109">Property</span></span>|<span data-ttu-id="66df9-110">Typ</span><span class="sxs-lookup"><span data-stu-id="66df9-110">Type</span></span>|<span data-ttu-id="66df9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66df9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66df9-112">url</span><span class="sxs-lookup"><span data-stu-id="66df9-112">url</span></span>|<span data-ttu-id="66df9-113">String</span><span class="sxs-lookup"><span data-stu-id="66df9-113">String</span></span>|<span data-ttu-id="66df9-114">URL für den Zugriff auf zulässige</span><span class="sxs-lookup"><span data-stu-id="66df9-114">URL allowed to access</span></span>|
|<span data-ttu-id="66df9-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="66df9-115">bookmarkFolder</span></span>|<span data-ttu-id="66df9-116">String</span><span class="sxs-lookup"><span data-stu-id="66df9-116">String</span></span>|<span data-ttu-id="66df9-117">Der Ordner, in dem die Textmarke in Safari hinzugefügt werden soll</span><span class="sxs-lookup"><span data-stu-id="66df9-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="66df9-118">displayName</span><span class="sxs-lookup"><span data-stu-id="66df9-118">displayName</span></span>|<span data-ttu-id="66df9-119">String</span><span class="sxs-lookup"><span data-stu-id="66df9-119">String</span></span>|<span data-ttu-id="66df9-120">Der Anzeigename der Textmarke</span><span class="sxs-lookup"><span data-stu-id="66df9-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="66df9-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="66df9-121">Relationships</span></span>
<span data-ttu-id="66df9-122">Keine</span><span class="sxs-lookup"><span data-stu-id="66df9-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="66df9-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66df9-123">JSON Representation</span></span>
<span data-ttu-id="66df9-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="66df9-124">Here is a JSON representation of the resource.</span></span>
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





