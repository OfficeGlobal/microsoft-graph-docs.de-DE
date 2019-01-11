---
title: androidMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine Android-App.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9cc203cc9268849e8b7b46d994c166378252df59
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871743"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="37dc9-103">androidMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="37dc9-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="37dc9-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="37dc9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37dc9-105">Der Bezeichner für eine Android-App.</span><span class="sxs-lookup"><span data-stu-id="37dc9-105">The identifier for an Android app.</span></span>

<span data-ttu-id="37dc9-106">Erbt von [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="37dc9-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="37dc9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="37dc9-107">Properties</span></span>
|<span data-ttu-id="37dc9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="37dc9-108">Property</span></span>|<span data-ttu-id="37dc9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="37dc9-109">Type</span></span>|<span data-ttu-id="37dc9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37dc9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37dc9-111">packageId</span><span class="sxs-lookup"><span data-stu-id="37dc9-111">packageId</span></span>|<span data-ttu-id="37dc9-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37dc9-112">String</span></span>|<span data-ttu-id="37dc9-113">Der Bezeichner für eine App wie im Play Store definiert.</span><span class="sxs-lookup"><span data-stu-id="37dc9-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37dc9-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="37dc9-114">Relationships</span></span>
<span data-ttu-id="37dc9-115">Keine</span><span class="sxs-lookup"><span data-stu-id="37dc9-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="37dc9-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="37dc9-116">JSON Representation</span></span>
<span data-ttu-id="37dc9-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="37dc9-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```



