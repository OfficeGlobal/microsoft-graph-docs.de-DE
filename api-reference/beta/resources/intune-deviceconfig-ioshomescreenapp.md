---
title: iosHomeScreenApp-Ressourcentyp
description: Gibt das Symbol einer App auf der Startseite an.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dcc90e774f8d032d46968fc4f751923bcc52e559
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412324"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="f6012-103">iosHomeScreenApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f6012-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="f6012-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f6012-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f6012-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6012-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6012-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6012-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6012-107">Gibt das Symbol einer App auf der Startseite an.</span><span class="sxs-lookup"><span data-stu-id="f6012-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="f6012-108">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="f6012-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f6012-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f6012-109">Properties</span></span>
|<span data-ttu-id="f6012-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f6012-110">Property</span></span>|<span data-ttu-id="f6012-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f6012-111">Type</span></span>|<span data-ttu-id="f6012-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6012-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6012-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f6012-113">displayName</span></span>|<span data-ttu-id="f6012-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6012-114">String</span></span>|<span data-ttu-id="f6012-115">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="f6012-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="f6012-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="f6012-116">bundleID</span></span>|<span data-ttu-id="f6012-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f6012-117">String</span></span>|<span data-ttu-id="f6012-118">Paket-ID der App</span><span class="sxs-lookup"><span data-stu-id="f6012-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6012-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f6012-119">Relationships</span></span>
<span data-ttu-id="f6012-120">Keine</span><span class="sxs-lookup"><span data-stu-id="f6012-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6012-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f6012-121">JSON Representation</span></span>
<span data-ttu-id="f6012-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f6012-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```




