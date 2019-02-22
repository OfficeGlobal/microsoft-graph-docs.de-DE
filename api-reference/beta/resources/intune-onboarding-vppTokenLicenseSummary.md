---
title: vppTokenLicenseSummary-Ressourcentyp
description: Lizenzzusammenfassung einer bestimmten app in einem Token.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f9c126323e0f5785752238ec64cfade2c34d5c24
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161061"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="9d5b5-103">vppTokenLicenseSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9d5b5-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="9d5b5-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9d5b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d5b5-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9d5b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d5b5-106">Lizenzzusammenfassung einer bestimmten app in einem Token.</span><span class="sxs-lookup"><span data-stu-id="9d5b5-106">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="9d5b5-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9d5b5-107">Properties</span></span>
|<span data-ttu-id="9d5b5-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9d5b5-108">Property</span></span>|<span data-ttu-id="9d5b5-109">Typ</span><span class="sxs-lookup"><span data-stu-id="9d5b5-109">Type</span></span>|<span data-ttu-id="9d5b5-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d5b5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d5b5-111">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="9d5b5-111">vppTokenId</span></span>|<span data-ttu-id="9d5b5-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9d5b5-112">String</span></span>|<span data-ttu-id="9d5b5-113">Bezeichner des VPP-Tokens.</span><span class="sxs-lookup"><span data-stu-id="9d5b5-113">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="9d5b5-114">appleId</span><span class="sxs-lookup"><span data-stu-id="9d5b5-114">appleId</span></span>|<span data-ttu-id="9d5b5-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9d5b5-115">String</span></span>|<span data-ttu-id="9d5b5-116">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="9d5b5-116">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="9d5b5-117">organizationName</span><span class="sxs-lookup"><span data-stu-id="9d5b5-117">organizationName</span></span>|<span data-ttu-id="9d5b5-118">String</span><span class="sxs-lookup"><span data-stu-id="9d5b5-118">String</span></span>|<span data-ttu-id="9d5b5-119">Die Organisation, die dem Apple Volume Purchase Program-Token zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="9d5b5-119">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="9d5b5-120">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="9d5b5-120">availableLicenseCount</span></span>|<span data-ttu-id="9d5b5-121">Int32</span><span class="sxs-lookup"><span data-stu-id="9d5b5-121">Int32</span></span>|<span data-ttu-id="9d5b5-122">Die Anzahl der verfügbaren VPP-Lizenzen.</span><span class="sxs-lookup"><span data-stu-id="9d5b5-122">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="9d5b5-123">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="9d5b5-123">usedLicenseCount</span></span>|<span data-ttu-id="9d5b5-124">Int32</span><span class="sxs-lookup"><span data-stu-id="9d5b5-124">Int32</span></span>|<span data-ttu-id="9d5b5-125">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="9d5b5-125">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d5b5-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9d5b5-126">Relationships</span></span>
<span data-ttu-id="9d5b5-127">Keine</span><span class="sxs-lookup"><span data-stu-id="9d5b5-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d5b5-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9d5b5-128">JSON Representation</span></span>
<span data-ttu-id="9d5b5-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9d5b5-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenLicenseSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenLicenseSummary",
  "vppTokenId": "String",
  "appleId": "String",
  "organizationName": "String",
  "availableLicenseCount": 1024,
  "usedLicenseCount": 1024
}
```




