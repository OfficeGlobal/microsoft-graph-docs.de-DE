---
title: Ressourcentyp securityVendorInformation
description: " SubProvider = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fb5dee36da08332fd5c36f7ee4e578cc9fb7deaa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945937"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="84d14-103">Ressourcentyp securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="84d14-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="84d14-104">Enthält Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="84d14-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="84d14-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="84d14-105">Properties</span></span>

| <span data-ttu-id="84d14-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="84d14-106">Property</span></span>   | <span data-ttu-id="84d14-107">Typ</span><span class="sxs-lookup"><span data-stu-id="84d14-107">Type</span></span>|<span data-ttu-id="84d14-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84d14-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84d14-109">Anbieter</span><span class="sxs-lookup"><span data-stu-id="84d14-109">provider</span></span> |<span data-ttu-id="84d14-110">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84d14-110">String</span></span>|<span data-ttu-id="84d14-111">Bestimmte Anbieter (Product/Service - nicht Hersteller Unternehmen); beispielsweise WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="84d14-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="84d14-112">providerVersion</span><span class="sxs-lookup"><span data-stu-id="84d14-112">providerVersion</span></span>|<span data-ttu-id="84d14-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84d14-113">String</span></span>|<span data-ttu-id="84d14-114">Version des Anbieters oder Subprovider, falls vorhanden, die Warnung ausgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="84d14-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="84d14-115">*Erforderlich*</span><span class="sxs-lookup"><span data-stu-id="84d14-115">*Required*</span></span>|
|<span data-ttu-id="84d14-116">subProvider</span><span class="sxs-lookup"><span data-stu-id="84d14-116">subProvider</span></span>|<span data-ttu-id="84d14-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84d14-117">String</span></span>|<span data-ttu-id="84d14-118">Bestimmte Subprovider (unter aggregieren Anbieter); beispielsweise WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="84d14-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="84d14-119">Hersteller</span><span class="sxs-lookup"><span data-stu-id="84d14-119">vendor</span></span> |<span data-ttu-id="84d14-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84d14-120">String</span></span>|<span data-ttu-id="84d14-121">Name des Herstellers alert (beispielsweise Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="84d14-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="84d14-122">*Erforderlich*</span><span class="sxs-lookup"><span data-stu-id="84d14-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="84d14-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="84d14-123">JSON representation</span></span>

<span data-ttu-id="84d14-124">Die folgenden ist eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="84d14-124">The folllowing is a JSON representation of the resource.</span></span>
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
