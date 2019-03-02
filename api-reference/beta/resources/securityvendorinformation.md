---
title: securityVendorInformation-Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 7f48c27ba94d8419ce244143a48cf6ab04dd080e
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30364584"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="7e249-104">securityVendorInformation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7e249-104">securityVendorInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e249-105">Enthält Details zum Sicherheitsprodukt/-Dienstanbieter,-Anbieter und-subprovider (beispielsweise Vendor = Microsoft; Provider = Windows Defender-ATP; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="7e249-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="7e249-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7e249-106">Properties</span></span>

| <span data-ttu-id="7e249-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7e249-107">Property</span></span>   | <span data-ttu-id="7e249-108">Typ</span><span class="sxs-lookup"><span data-stu-id="7e249-108">Type</span></span>|<span data-ttu-id="7e249-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7e249-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e249-110">Anbieter</span><span class="sxs-lookup"><span data-stu-id="7e249-110">provider</span></span> |<span data-ttu-id="7e249-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e249-111">String</span></span>|<span data-ttu-id="7e249-112">Bestimmter Anbieter (Product/Service-not Vendor Company); Beispiel: WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="7e249-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="7e249-113">Provider Version</span><span class="sxs-lookup"><span data-stu-id="7e249-113">providerVersion</span></span>|<span data-ttu-id="7e249-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e249-114">String</span></span>|<span data-ttu-id="7e249-115">Die Version des Anbieters oder subproviders, sofern vorhanden, die die Warnung generiert hat.</span><span class="sxs-lookup"><span data-stu-id="7e249-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="7e249-116">**Erforderlich**</span><span class="sxs-lookup"><span data-stu-id="7e249-116">**Required**</span></span>|
|<span data-ttu-id="7e249-117">Sekundären Anbieter</span><span class="sxs-lookup"><span data-stu-id="7e249-117">subProvider</span></span>|<span data-ttu-id="7e249-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e249-118">String</span></span>|<span data-ttu-id="7e249-119">Bestimmter subprovider (unter Aggregations Anbieter); Beispiel: WindowsDefenderATP. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="7e249-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="7e249-120">Hersteller</span><span class="sxs-lookup"><span data-stu-id="7e249-120">vendor</span></span> |<span data-ttu-id="7e249-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7e249-121">String</span></span>|<span data-ttu-id="7e249-122">Name des Warnungs Anbieters (beispielsweise Microsoft, Dell, FireEye arbeitete).</span><span class="sxs-lookup"><span data-stu-id="7e249-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="7e249-123">**Erforderlich**</span><span class="sxs-lookup"><span data-stu-id="7e249-123">**Required**</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7e249-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7e249-124">JSON representation</span></span>

<span data-ttu-id="7e249-125">Folllowing ist eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7e249-125">The folllowing is a JSON representation of the resource.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securityvendorinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
