---
title: iosHomeScreenPage-Ressourcentyp
description: Eine Seite mit Apps und Ordnern auf der Startseite.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b2b6e4ba9cc70253e929a0f434a292aeafd24bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398548"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="5145c-103">iosHomeScreenPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="5145c-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="5145c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5145c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5145c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5145c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5145c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5145c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5145c-107">Eine Seite mit Apps und Ordnern auf der Startseite.</span><span class="sxs-lookup"><span data-stu-id="5145c-107">A page containing apps and folders on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="5145c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5145c-108">Properties</span></span>
|<span data-ttu-id="5145c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5145c-109">Property</span></span>|<span data-ttu-id="5145c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="5145c-110">Type</span></span>|<span data-ttu-id="5145c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5145c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5145c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5145c-112">displayName</span></span>|<span data-ttu-id="5145c-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5145c-113">String</span></span>|<span data-ttu-id="5145c-114">Name der Seite</span><span class="sxs-lookup"><span data-stu-id="5145c-114">Name of the page</span></span>|
|<span data-ttu-id="5145c-115">Symbole</span><span class="sxs-lookup"><span data-stu-id="5145c-115">icons</span></span>|<span data-ttu-id="5145c-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="5145c-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="5145c-117">Eine Liste der Apps und Ordner, die auf einer Seite angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="5145c-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="5145c-118">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="5145c-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5145c-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="5145c-119">Relationships</span></span>
<span data-ttu-id="5145c-120">Keine</span><span class="sxs-lookup"><span data-stu-id="5145c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5145c-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5145c-121">JSON Representation</span></span>
<span data-ttu-id="5145c-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="5145c-122">Here is a JSON representation of the resource.</span></span>
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




