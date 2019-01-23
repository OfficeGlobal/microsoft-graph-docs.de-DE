---
title: iosHomeScreenFolder-Ressourcentyp
description: Ein Ordner mit App-Seiten auf der Startseite
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 36ea4a00b9310623027179e1d6d2e1c64888c470
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407508"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="9df37-103">iosHomeScreenFolder-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9df37-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="9df37-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9df37-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9df37-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9df37-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9df37-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9df37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9df37-107">Ein Ordner mit App-Seiten auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="9df37-107">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="9df37-108">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="9df37-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9df37-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9df37-109">Properties</span></span>
|<span data-ttu-id="9df37-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9df37-110">Property</span></span>|<span data-ttu-id="9df37-111">Typ</span><span class="sxs-lookup"><span data-stu-id="9df37-111">Type</span></span>|<span data-ttu-id="9df37-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9df37-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9df37-113">displayName</span><span class="sxs-lookup"><span data-stu-id="9df37-113">displayName</span></span>|<span data-ttu-id="9df37-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9df37-114">String</span></span>|<span data-ttu-id="9df37-115">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="9df37-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="9df37-116">Seiten</span><span class="sxs-lookup"><span data-stu-id="9df37-116">pages</span></span>|<span data-ttu-id="9df37-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9df37-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="9df37-118">Seiten mit Startbildschirm-Layout-Symbolen, die dem Anwendungstyp entsprechen müssen.</span><span class="sxs-lookup"><span data-stu-id="9df37-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="9df37-119">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="9df37-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9df37-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9df37-120">Relationships</span></span>
<span data-ttu-id="9df37-121">Keine</span><span class="sxs-lookup"><span data-stu-id="9df37-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9df37-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9df37-122">JSON Representation</span></span>
<span data-ttu-id="9df37-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9df37-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
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
```




