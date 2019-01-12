---
title: Ressourcentyp securityVendorInformation
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 0137abd7a9df0df94f73e18d7efa201008031ff6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939924"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="56cb2-104">Ressourcentyp securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="56cb2-104">securityVendorInformation resource type</span></span>

 > <span data-ttu-id="56cb2-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="56cb2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56cb2-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56cb2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56cb2-107">Enthält Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="56cb2-107">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="56cb2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="56cb2-108">Properties</span></span>

| <span data-ttu-id="56cb2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56cb2-109">Property</span></span>   | <span data-ttu-id="56cb2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="56cb2-110">Type</span></span>|<span data-ttu-id="56cb2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56cb2-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56cb2-112">Anbieter</span><span class="sxs-lookup"><span data-stu-id="56cb2-112">provider</span></span> |<span data-ttu-id="56cb2-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56cb2-113">String</span></span>|<span data-ttu-id="56cb2-114">Bestimmte Anbieter (Product/Service - nicht Hersteller Unternehmen); beispielsweise WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="56cb2-114">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="56cb2-115">providerVersion</span><span class="sxs-lookup"><span data-stu-id="56cb2-115">providerVersion</span></span>|<span data-ttu-id="56cb2-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56cb2-116">String</span></span>|<span data-ttu-id="56cb2-117">Version des Anbieters oder Subprovider, falls vorhanden, die Warnung ausgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="56cb2-117">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="56cb2-118">*Erforderlich*</span><span class="sxs-lookup"><span data-stu-id="56cb2-118">*Required*</span></span>|
|<span data-ttu-id="56cb2-119">subProvider</span><span class="sxs-lookup"><span data-stu-id="56cb2-119">subProvider</span></span>|<span data-ttu-id="56cb2-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56cb2-120">String</span></span>|<span data-ttu-id="56cb2-121">Bestimmte Subprovider (unter aggregieren Anbieter); beispielsweise WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="56cb2-121">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="56cb2-122">Hersteller</span><span class="sxs-lookup"><span data-stu-id="56cb2-122">vendor</span></span> |<span data-ttu-id="56cb2-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56cb2-123">String</span></span>|<span data-ttu-id="56cb2-124">Name des Herstellers alert (beispielsweise Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="56cb2-124">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="56cb2-125">*Erforderlich*</span><span class="sxs-lookup"><span data-stu-id="56cb2-125">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56cb2-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="56cb2-126">JSON representation</span></span>

<span data-ttu-id="56cb2-127">Die folgenden ist eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="56cb2-127">The folllowing is a JSON representation of the resource.</span></span>
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
