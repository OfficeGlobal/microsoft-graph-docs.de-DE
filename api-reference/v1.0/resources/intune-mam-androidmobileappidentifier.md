---
title: androidMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine Android-App.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa3a0f90626ea01290ccd1d0eee3873374efb546
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261173"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="12497-103">androidMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="12497-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="12497-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="12497-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12497-105">Der Bezeichner für eine Android-App.</span><span class="sxs-lookup"><span data-stu-id="12497-105">The identifier for an Android app.</span></span>


<span data-ttu-id="12497-106">Erbt von [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="12497-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="12497-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="12497-107">Properties</span></span>
|<span data-ttu-id="12497-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="12497-108">Property</span></span>|<span data-ttu-id="12497-109">Typ</span><span class="sxs-lookup"><span data-stu-id="12497-109">Type</span></span>|<span data-ttu-id="12497-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12497-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12497-111">packageId</span><span class="sxs-lookup"><span data-stu-id="12497-111">packageId</span></span>|<span data-ttu-id="12497-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="12497-112">String</span></span>|<span data-ttu-id="12497-113">Der Bezeichner für eine App wie im Play Store definiert.</span><span class="sxs-lookup"><span data-stu-id="12497-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12497-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="12497-114">Relationships</span></span>
<span data-ttu-id="12497-115">Keine</span><span class="sxs-lookup"><span data-stu-id="12497-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12497-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="12497-116">JSON Representation</span></span>
<span data-ttu-id="12497-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="12497-117">Here is a JSON representation of the resource.</span></span>
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



