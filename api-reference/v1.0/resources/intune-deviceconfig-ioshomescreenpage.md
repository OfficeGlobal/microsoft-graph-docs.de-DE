---
title: iosHomeScreenPage-Ressourcentyp
description: Eine Seite mit Apps und Ordnern auf der Startseite.
author: tfitzmac
ms.openlocfilehash: b8aca5c671d0c8521cdf8a870a2f0ad3cd35ba1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321462"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="0d935-103">iosHomeScreenPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0d935-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="0d935-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0d935-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0d935-105">Eine Seite mit Apps und Ordnern auf der Startseite.</span><span class="sxs-lookup"><span data-stu-id="0d935-105">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="0d935-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0d935-106">Properties</span></span>
|<span data-ttu-id="0d935-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0d935-107">Property</span></span>|<span data-ttu-id="0d935-108">Typ</span><span class="sxs-lookup"><span data-stu-id="0d935-108">Type</span></span>|<span data-ttu-id="0d935-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0d935-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d935-110">displayName</span><span class="sxs-lookup"><span data-stu-id="0d935-110">displayName</span></span>|<span data-ttu-id="0d935-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0d935-111">String</span></span>|<span data-ttu-id="0d935-112">Name der Seite</span><span class="sxs-lookup"><span data-stu-id="0d935-112">Name of the page</span></span>|
|<span data-ttu-id="0d935-113">Symbole</span><span class="sxs-lookup"><span data-stu-id="0d935-113">icons</span></span>|<span data-ttu-id="0d935-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="0d935-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="0d935-115">Eine Liste der Apps und Ordner, die auf einer Seite angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="0d935-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="0d935-116">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="0d935-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d935-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0d935-117">Relationships</span></span>
<span data-ttu-id="0d935-118">Keine</span><span class="sxs-lookup"><span data-stu-id="0d935-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0d935-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0d935-119">JSON Representation</span></span>
<span data-ttu-id="0d935-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0d935-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenItem",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```



