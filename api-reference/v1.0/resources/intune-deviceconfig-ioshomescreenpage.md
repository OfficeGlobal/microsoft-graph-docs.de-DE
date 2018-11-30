---
title: iosHomeScreenPage-Ressourcentyp
description: Eine Seite mit Apps und Ordnern auf der Startseite.
ms.openlocfilehash: 4ef336bc104a203739904b67e301b489627e7ff1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017600"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="fdceb-103">iosHomeScreenPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fdceb-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="fdceb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fdceb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fdceb-105">Eine Seite mit Apps und Ordnern auf der Startseite.</span><span class="sxs-lookup"><span data-stu-id="fdceb-105">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="fdceb-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fdceb-106">Properties</span></span>
|<span data-ttu-id="fdceb-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fdceb-107">Property</span></span>|<span data-ttu-id="fdceb-108">Typ</span><span class="sxs-lookup"><span data-stu-id="fdceb-108">Type</span></span>|<span data-ttu-id="fdceb-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fdceb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdceb-110">displayName</span><span class="sxs-lookup"><span data-stu-id="fdceb-110">displayName</span></span>|<span data-ttu-id="fdceb-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fdceb-111">String</span></span>|<span data-ttu-id="fdceb-112">Name der Seite</span><span class="sxs-lookup"><span data-stu-id="fdceb-112">Name of the page</span></span>|
|<span data-ttu-id="fdceb-113">Symbole</span><span class="sxs-lookup"><span data-stu-id="fdceb-113">icons</span></span>|<span data-ttu-id="fdceb-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="fdceb-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="fdceb-115">Eine Liste der Apps und Ordner, die auf einer Seite angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="fdceb-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="fdceb-116">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="fdceb-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fdceb-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fdceb-117">Relationships</span></span>
<span data-ttu-id="fdceb-118">Keine</span><span class="sxs-lookup"><span data-stu-id="fdceb-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fdceb-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fdceb-119">JSON Representation</span></span>
<span data-ttu-id="fdceb-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fdceb-120">Here is a JSON representation of the resource.</span></span>
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



