---
title: iosHomeScreenPage-Ressourcentyp
description: Eine Seite mit Apps und Ordnern auf der Startseite.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c958570caa81cff7add1e174cbb678fc68cecd87
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149539"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="a75bf-103">iosHomeScreenPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a75bf-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="a75bf-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a75bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a75bf-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a75bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a75bf-106">Eine Seite mit Apps und Ordnern auf der Startseite.</span><span class="sxs-lookup"><span data-stu-id="a75bf-106">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="a75bf-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a75bf-107">Properties</span></span>
|<span data-ttu-id="a75bf-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a75bf-108">Property</span></span>|<span data-ttu-id="a75bf-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a75bf-109">Type</span></span>|<span data-ttu-id="a75bf-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a75bf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a75bf-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a75bf-111">displayName</span></span>|<span data-ttu-id="a75bf-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a75bf-112">String</span></span>|<span data-ttu-id="a75bf-113">Name der Seite</span><span class="sxs-lookup"><span data-stu-id="a75bf-113">Name of the page</span></span>|
|<span data-ttu-id="a75bf-114">Symbole</span><span class="sxs-lookup"><span data-stu-id="a75bf-114">icons</span></span>|<span data-ttu-id="a75bf-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a75bf-115">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="a75bf-116">Eine Liste der Apps und Ordner, die auf einer Seite angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="a75bf-116">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="a75bf-117">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="a75bf-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a75bf-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a75bf-118">Relationships</span></span>
<span data-ttu-id="a75bf-119">Keine</span><span class="sxs-lookup"><span data-stu-id="a75bf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a75bf-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a75bf-120">JSON Representation</span></span>
<span data-ttu-id="a75bf-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a75bf-121">Here is a JSON representation of the resource.</span></span>
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




