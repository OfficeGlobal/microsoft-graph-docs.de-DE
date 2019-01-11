---
title: iosHomeScreenApp-Ressourcentyp
description: Gibt das Symbol einer App auf der Startseite an.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 39db8de19fbfc568f85c4930e8c3124ffea2dd57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850596"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="dadf2-103">iosHomeScreenApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="dadf2-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="dadf2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dadf2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dadf2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dadf2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dadf2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dadf2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dadf2-107">Gibt das Symbol einer App auf der Startseite an.</span><span class="sxs-lookup"><span data-stu-id="dadf2-107">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="dadf2-108">Erbt von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="dadf2-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dadf2-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="dadf2-109">Properties</span></span>
|<span data-ttu-id="dadf2-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="dadf2-110">Property</span></span>|<span data-ttu-id="dadf2-111">Typ</span><span class="sxs-lookup"><span data-stu-id="dadf2-111">Type</span></span>|<span data-ttu-id="dadf2-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="dadf2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dadf2-113">displayName</span><span class="sxs-lookup"><span data-stu-id="dadf2-113">displayName</span></span>|<span data-ttu-id="dadf2-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dadf2-114">String</span></span>|<span data-ttu-id="dadf2-115">Name der von [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) geerbten App</span><span class="sxs-lookup"><span data-stu-id="dadf2-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="dadf2-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="dadf2-116">bundleID</span></span>|<span data-ttu-id="dadf2-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="dadf2-117">String</span></span>|<span data-ttu-id="dadf2-118">Paket-ID der App</span><span class="sxs-lookup"><span data-stu-id="dadf2-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="dadf2-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="dadf2-119">Relationships</span></span>
<span data-ttu-id="dadf2-120">Keine</span><span class="sxs-lookup"><span data-stu-id="dadf2-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dadf2-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="dadf2-121">JSON Representation</span></span>
<span data-ttu-id="dadf2-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="dadf2-122">Here is a JSON representation of the resource.</span></span>
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





