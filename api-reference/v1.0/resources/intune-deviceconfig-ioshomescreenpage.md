---
title: iosHomeScreenPage-Ressourcentyp
description: Eine Seite mit Apps und Ordnern auf der Startseite.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4317ac80e7ff6273b809eb747da745f5cf5edb6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254387"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="61d6d-103">iosHomeScreenPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="61d6d-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="61d6d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="61d6d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61d6d-105">Eine Seite mit Apps und Ordnern auf der Startseite.</span><span class="sxs-lookup"><span data-stu-id="61d6d-105">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="61d6d-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="61d6d-106">Properties</span></span>
|<span data-ttu-id="61d6d-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61d6d-107">Property</span></span>|<span data-ttu-id="61d6d-108">Typ</span><span class="sxs-lookup"><span data-stu-id="61d6d-108">Type</span></span>|<span data-ttu-id="61d6d-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61d6d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61d6d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="61d6d-110">displayName</span></span>|<span data-ttu-id="61d6d-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61d6d-111">String</span></span>|<span data-ttu-id="61d6d-112">Name der Seite</span><span class="sxs-lookup"><span data-stu-id="61d6d-112">Name of the page</span></span>|
|<span data-ttu-id="61d6d-113">Symbole</span><span class="sxs-lookup"><span data-stu-id="61d6d-113">icons</span></span>|<span data-ttu-id="61d6d-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="61d6d-114">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="61d6d-115">Eine Liste der Apps und Ordner, die auf einer Seite angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="61d6d-115">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="61d6d-116">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="61d6d-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61d6d-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="61d6d-117">Relationships</span></span>
<span data-ttu-id="61d6d-118">Keine</span><span class="sxs-lookup"><span data-stu-id="61d6d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61d6d-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="61d6d-119">JSON Representation</span></span>
<span data-ttu-id="61d6d-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="61d6d-120">Here is a JSON representation of the resource.</span></span>
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



