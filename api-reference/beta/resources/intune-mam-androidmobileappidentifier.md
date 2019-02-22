---
title: androidMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine Android-App.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a45c31a7829102dfabee85f930be397dede17513
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140103"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="8bb1c-103">androidMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8bb1c-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="8bb1c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8bb1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bb1c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="8bb1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bb1c-106">Der Bezeichner für eine Android-App.</span><span class="sxs-lookup"><span data-stu-id="8bb1c-106">The identifier for an Android app.</span></span>


<span data-ttu-id="8bb1c-107">Erbt von [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="8bb1c-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8bb1c-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8bb1c-108">Properties</span></span>
|<span data-ttu-id="8bb1c-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8bb1c-109">Property</span></span>|<span data-ttu-id="8bb1c-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8bb1c-110">Type</span></span>|<span data-ttu-id="8bb1c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8bb1c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bb1c-112">packageId</span><span class="sxs-lookup"><span data-stu-id="8bb1c-112">packageId</span></span>|<span data-ttu-id="8bb1c-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8bb1c-113">String</span></span>|<span data-ttu-id="8bb1c-114">Der Bezeichner für eine App wie im Play Store definiert.</span><span class="sxs-lookup"><span data-stu-id="8bb1c-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bb1c-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8bb1c-115">Relationships</span></span>
<span data-ttu-id="8bb1c-116">Keine</span><span class="sxs-lookup"><span data-stu-id="8bb1c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bb1c-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8bb1c-117">JSON Representation</span></span>
<span data-ttu-id="8bb1c-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8bb1c-118">Here is a JSON representation of the resource.</span></span>
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




