---
title: iosMobileAppIdentifier-Ressourcentyp
description: Der Bezeichner für eine iOS-App.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ddd09f6d1f0d49b00282c55bfa6dcbef1fcb1d2c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409930"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="2e266-103">iosMobileAppIdentifier-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="2e266-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="2e266-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="2e266-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2e266-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2e266-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e266-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2e266-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e266-107">Der Bezeichner für eine iOS-App.</span><span class="sxs-lookup"><span data-stu-id="2e266-107">The identifier for an iOS app.</span></span>


<span data-ttu-id="2e266-108">Erbt von [MobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="2e266-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e266-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2e266-109">Properties</span></span>
|<span data-ttu-id="2e266-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2e266-110">Property</span></span>|<span data-ttu-id="2e266-111">Typ</span><span class="sxs-lookup"><span data-stu-id="2e266-111">Type</span></span>|<span data-ttu-id="2e266-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2e266-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e266-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="2e266-113">bundleId</span></span>|<span data-ttu-id="2e266-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2e266-114">String</span></span>|<span data-ttu-id="2e266-115">Der Bezeichner für eine App wie im App-Store definiert.</span><span class="sxs-lookup"><span data-stu-id="2e266-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e266-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2e266-116">Relationships</span></span>
<span data-ttu-id="2e266-117">Keine</span><span class="sxs-lookup"><span data-stu-id="2e266-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e266-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2e266-118">JSON Representation</span></span>
<span data-ttu-id="2e266-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2e266-119">Here is a JSON representation of the resource.</span></span>
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




