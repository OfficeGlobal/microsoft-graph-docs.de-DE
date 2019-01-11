---
title: iosHomeScreenPage-Ressourcentyp
description: Eine Seite mit Apps und Ordnern auf der Startseite.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2dab636fb4e1793916b1408007bc56aaaa3933a1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855230"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="831ba-103">iosHomeScreenPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="831ba-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="831ba-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="831ba-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="831ba-105">Eine Seite mit Apps und Ordnern auf der Startseite.</span><span class="sxs-lookup"><span data-stu-id="831ba-105">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="831ba-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="831ba-106">Properties</span></span>
|<span data-ttu-id="831ba-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="831ba-107">Property</span></span>|<span data-ttu-id="831ba-108">Typ</span><span class="sxs-lookup"><span data-stu-id="831ba-108">Type</span></span>|<span data-ttu-id="831ba-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="831ba-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="831ba-110">displayName</span><span class="sxs-lookup"><span data-stu-id="831ba-110">displayName</span></span>|<span data-ttu-id="831ba-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="831ba-111">String</span></span>|<span data-ttu-id="831ba-112">Name der Seite</span><span class="sxs-lookup"><span data-stu-id="831ba-112">Name of the page</span></span>|
|<span data-ttu-id="831ba-113">Symbole</span><span class="sxs-lookup"><span data-stu-id="831ba-113">icons</span></span>|<span data-ttu-id="831ba-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="831ba-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="831ba-115">Eine Liste der Apps und Ordner, die auf einer Seite angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="831ba-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="831ba-116">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="831ba-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="831ba-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="831ba-117">Relationships</span></span>
<span data-ttu-id="831ba-118">Keine</span><span class="sxs-lookup"><span data-stu-id="831ba-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="831ba-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="831ba-119">JSON Representation</span></span>
<span data-ttu-id="831ba-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="831ba-120">Here is a JSON representation of the resource.</span></span>
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



