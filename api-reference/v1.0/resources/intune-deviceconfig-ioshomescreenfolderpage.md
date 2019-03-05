---
title: iosHomeScreenFolderPage-Ressourcentyp
description: Ein Ordner mit Apps auf der Startseite
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f00c67b7a0679d92ef6aac78bc0317e461dcd2f9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255493"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="66b89-103">iosHomeScreenFolderPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="66b89-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="66b89-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="66b89-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66b89-105">Ein Ordner mit Apps auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="66b89-105">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="66b89-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="66b89-106">Properties</span></span>
|<span data-ttu-id="66b89-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="66b89-107">Property</span></span>|<span data-ttu-id="66b89-108">Typ</span><span class="sxs-lookup"><span data-stu-id="66b89-108">Type</span></span>|<span data-ttu-id="66b89-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="66b89-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66b89-110">displayName</span><span class="sxs-lookup"><span data-stu-id="66b89-110">displayName</span></span>|<span data-ttu-id="66b89-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="66b89-111">String</span></span>|<span data-ttu-id="66b89-112">Name des Ordnerseite</span><span class="sxs-lookup"><span data-stu-id="66b89-112">Name of the folder page</span></span>|
|<span data-ttu-id="66b89-113">Apps</span><span class="sxs-lookup"><span data-stu-id="66b89-113">apps</span></span>|<span data-ttu-id="66b89-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="66b89-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="66b89-115">Eine Liste der Apps, die auf einer Seite innerhalb eines Ordners angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="66b89-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="66b89-116">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="66b89-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66b89-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="66b89-117">Relationships</span></span>
<span data-ttu-id="66b89-118">Keine</span><span class="sxs-lookup"><span data-stu-id="66b89-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66b89-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="66b89-119">JSON Representation</span></span>
<span data-ttu-id="66b89-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="66b89-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```



