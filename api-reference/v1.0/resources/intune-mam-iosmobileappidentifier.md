---
title: iosMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine iOS-App.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb0eaade90c88cc553072f30dd36c42db4f44513
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30249963"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="48f9e-103">iosMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="48f9e-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="48f9e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="48f9e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48f9e-105">Der Bezeichner für eine iOS-App.</span><span class="sxs-lookup"><span data-stu-id="48f9e-105">The identifier for an iOS app.</span></span>


<span data-ttu-id="48f9e-106">Erbt von [MobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="48f9e-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="48f9e-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="48f9e-107">Properties</span></span>
|<span data-ttu-id="48f9e-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="48f9e-108">Property</span></span>|<span data-ttu-id="48f9e-109">Typ</span><span class="sxs-lookup"><span data-stu-id="48f9e-109">Type</span></span>|<span data-ttu-id="48f9e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="48f9e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48f9e-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="48f9e-111">bundleId</span></span>|<span data-ttu-id="48f9e-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="48f9e-112">String</span></span>|<span data-ttu-id="48f9e-113">Der Bezeichner für eine App wie im App-Store definiert.</span><span class="sxs-lookup"><span data-stu-id="48f9e-113">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48f9e-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="48f9e-114">Relationships</span></span>
<span data-ttu-id="48f9e-115">Keine</span><span class="sxs-lookup"><span data-stu-id="48f9e-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48f9e-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="48f9e-116">JSON Representation</span></span>
<span data-ttu-id="48f9e-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="48f9e-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```



