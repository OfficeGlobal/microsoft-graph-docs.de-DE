---
title: Ressourcentyp securityVendorInformation
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e67a5306b1dd08933877dbe3e64cab766ccd6a96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512178"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="484ac-104">Ressourcentyp securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="484ac-104">securityVendorInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="484ac-105">Enthält Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="484ac-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="484ac-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="484ac-106">Properties</span></span>

| <span data-ttu-id="484ac-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="484ac-107">Property</span></span>   | <span data-ttu-id="484ac-108">Typ</span><span class="sxs-lookup"><span data-stu-id="484ac-108">Type</span></span>|<span data-ttu-id="484ac-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="484ac-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="484ac-110">Provider</span><span class="sxs-lookup"><span data-stu-id="484ac-110">provider</span></span> |<span data-ttu-id="484ac-111">String</span><span class="sxs-lookup"><span data-stu-id="484ac-111">String</span></span>|<span data-ttu-id="484ac-112">Bestimmte Anbieter (Product/Service - nicht Hersteller Unternehmen); beispielsweise WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="484ac-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="484ac-113">providerVersion</span><span class="sxs-lookup"><span data-stu-id="484ac-113">providerVersion</span></span>|<span data-ttu-id="484ac-114">String</span><span class="sxs-lookup"><span data-stu-id="484ac-114">String</span></span>|<span data-ttu-id="484ac-115">Version des Anbieters oder Subprovider, falls vorhanden, die Warnung ausgelöst wurde.</span><span class="sxs-lookup"><span data-stu-id="484ac-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="484ac-116">*Erforderlich*</span><span class="sxs-lookup"><span data-stu-id="484ac-116">*Required*</span></span>|
|<span data-ttu-id="484ac-117">subProvider</span><span class="sxs-lookup"><span data-stu-id="484ac-117">subProvider</span></span>|<span data-ttu-id="484ac-118">String</span><span class="sxs-lookup"><span data-stu-id="484ac-118">String</span></span>|<span data-ttu-id="484ac-119">Bestimmte Subprovider (unter aggregieren Anbieter); beispielsweise WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="484ac-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="484ac-120">Hersteller</span><span class="sxs-lookup"><span data-stu-id="484ac-120">vendor</span></span> |<span data-ttu-id="484ac-121">String</span><span class="sxs-lookup"><span data-stu-id="484ac-121">String</span></span>|<span data-ttu-id="484ac-122">Name des Herstellers alert (beispielsweise Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="484ac-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="484ac-123">*Erforderlich*</span><span class="sxs-lookup"><span data-stu-id="484ac-123">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="484ac-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="484ac-124">JSON representation</span></span>

<span data-ttu-id="484ac-125">Die folgenden ist eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="484ac-125">The folllowing is a JSON representation of the resource.</span></span>
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
