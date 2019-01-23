---
title: iosHomeScreenFolderPage-Ressourcentyp
description: Ein Ordner mit Apps auf der Startseite
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fa9462f8fb0640584515d1c209abd03de0e6200
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424175"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="50f97-103">iosHomeScreenFolderPage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="50f97-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="50f97-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="50f97-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="50f97-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50f97-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50f97-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="50f97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50f97-107">Ein Ordner mit Apps auf der Startseite</span><span class="sxs-lookup"><span data-stu-id="50f97-107">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="50f97-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="50f97-108">Properties</span></span>
|<span data-ttu-id="50f97-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50f97-109">Property</span></span>|<span data-ttu-id="50f97-110">Typ</span><span class="sxs-lookup"><span data-stu-id="50f97-110">Type</span></span>|<span data-ttu-id="50f97-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50f97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50f97-112">displayName</span><span class="sxs-lookup"><span data-stu-id="50f97-112">displayName</span></span>|<span data-ttu-id="50f97-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50f97-113">String</span></span>|<span data-ttu-id="50f97-114">Name des Ordnerseite</span><span class="sxs-lookup"><span data-stu-id="50f97-114">Name of the folder page</span></span>|
|<span data-ttu-id="50f97-115">Apps</span><span class="sxs-lookup"><span data-stu-id="50f97-115">apps</span></span>|<span data-ttu-id="50f97-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="50f97-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="50f97-117">Eine Liste der Apps, die auf einer Seite innerhalb eines Ordners angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="50f97-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="50f97-118">Diese Sammlung kann bis zu 500 Elemente enthalten.</span><span class="sxs-lookup"><span data-stu-id="50f97-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50f97-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="50f97-119">Relationships</span></span>
<span data-ttu-id="50f97-120">Keine</span><span class="sxs-lookup"><span data-stu-id="50f97-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50f97-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="50f97-121">JSON Representation</span></span>
<span data-ttu-id="50f97-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="50f97-122">Here is a JSON representation of the resource.</span></span>
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




