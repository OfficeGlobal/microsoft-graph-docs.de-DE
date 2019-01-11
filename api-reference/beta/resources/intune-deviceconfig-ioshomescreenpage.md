---
title: iosHomeScreenPage-Ressourcentyp
description: Eine Seite mit Apps und Ordnern auf der Startseite.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9425edb3fb330f8dc8bb445f34295433eea49712
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872793"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="162ea-103">iosHomeScreenPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="162ea-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="162ea-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="162ea-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="162ea-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="162ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="162ea-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="162ea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="162ea-107">Eine Seite mit Apps und Ordnern auf der Startseite.</span><span class="sxs-lookup"><span data-stu-id="162ea-107">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="162ea-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="162ea-108">Properties</span></span>
|<span data-ttu-id="162ea-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="162ea-109">Property</span></span>|<span data-ttu-id="162ea-110">Typ</span><span class="sxs-lookup"><span data-stu-id="162ea-110">Type</span></span>|<span data-ttu-id="162ea-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="162ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="162ea-112">displayName</span><span class="sxs-lookup"><span data-stu-id="162ea-112">displayName</span></span>|<span data-ttu-id="162ea-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="162ea-113">String</span></span>|<span data-ttu-id="162ea-114">Name der Seite</span><span class="sxs-lookup"><span data-stu-id="162ea-114">Name of the page</span></span>|
|<span data-ttu-id="162ea-115">Symbole</span><span class="sxs-lookup"><span data-stu-id="162ea-115">icons</span></span>|<span data-ttu-id="162ea-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="162ea-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="162ea-117">Eine Liste der Apps und Ordner, die auf einer Seite angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="162ea-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="162ea-118">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="162ea-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="162ea-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="162ea-119">Relationships</span></span>
<span data-ttu-id="162ea-120">Keine</span><span class="sxs-lookup"><span data-stu-id="162ea-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="162ea-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="162ea-121">JSON Representation</span></span>
<span data-ttu-id="162ea-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="162ea-122">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
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





