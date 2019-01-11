---
title: Ressourcentyp securityVendorInformation
description: " SubProvider = AppLocker)."
localization_priority: Normal
ms.openlocfilehash: e9d8551c085c05007388bf0c6e33143994c6969b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820146"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="896d3-103">Ressourcentyp securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="896d3-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="896d3-104">Enthält Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="896d3-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="896d3-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="896d3-105">Properties</span></span>

| <span data-ttu-id="896d3-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="896d3-106">Property</span></span>   | <span data-ttu-id="896d3-107">Typ</span><span class="sxs-lookup"><span data-stu-id="896d3-107">Type</span></span>|<span data-ttu-id="896d3-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="896d3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="896d3-109">Anbieter</span><span class="sxs-lookup"><span data-stu-id="896d3-109">provider</span></span> |<span data-ttu-id="896d3-110">String</span><span class="sxs-lookup"><span data-stu-id="896d3-110">String</span></span>|<span data-ttu-id="896d3-111">Bestimmte Anbieter (Product/Service - nicht Hersteller Unternehmen); beispielsweise WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="896d3-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="896d3-112">providerVersion</span><span class="sxs-lookup"><span data-stu-id="896d3-112">providerVersion</span></span>|<span data-ttu-id="896d3-113">String</span><span class="sxs-lookup"><span data-stu-id="896d3-113">String</span></span>|<span data-ttu-id="896d3-114">Version des Anbieters oder Subprovider, falls vorhanden, die Warnung ausgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="896d3-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="896d3-115">*Erforderlich*</span><span class="sxs-lookup"><span data-stu-id="896d3-115">*Required*</span></span>|
|<span data-ttu-id="896d3-116">subProvider</span><span class="sxs-lookup"><span data-stu-id="896d3-116">subProvider</span></span>|<span data-ttu-id="896d3-117">String</span><span class="sxs-lookup"><span data-stu-id="896d3-117">String</span></span>|<span data-ttu-id="896d3-118">Bestimmte Subprovider (unter aggregieren Anbieter); beispielsweise WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="896d3-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="896d3-119">Hersteller</span><span class="sxs-lookup"><span data-stu-id="896d3-119">vendor</span></span> |<span data-ttu-id="896d3-120">String</span><span class="sxs-lookup"><span data-stu-id="896d3-120">String</span></span>|<span data-ttu-id="896d3-121">Name des Herstellers alert (beispielsweise Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="896d3-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="896d3-122">*Erforderlich*</span><span class="sxs-lookup"><span data-stu-id="896d3-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="896d3-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="896d3-123">JSON representation</span></span>

<span data-ttu-id="896d3-124">Die folgenden ist eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="896d3-124">The folllowing is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
