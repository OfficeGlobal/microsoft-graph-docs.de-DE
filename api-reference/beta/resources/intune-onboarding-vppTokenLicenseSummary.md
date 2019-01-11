---
title: Ressourcentyp vppTokenLicenseSummary
description: Lizenz-Zusammenfassung der eine bestimmte app in einem Token.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e5972341aa3b390ae226d19f7d85fe918345c627
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824864"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="a9def-103">Ressourcentyp vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="a9def-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="a9def-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a9def-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9def-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a9def-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9def-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a9def-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9def-107">Lizenz-Zusammenfassung der eine bestimmte app in einem Token.</span><span class="sxs-lookup"><span data-stu-id="a9def-107">License summary of a given app in a token.</span></span>
## <a name="properties"></a><span data-ttu-id="a9def-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a9def-108">Properties</span></span>
|<span data-ttu-id="a9def-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a9def-109">Property</span></span>|<span data-ttu-id="a9def-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a9def-110">Type</span></span>|<span data-ttu-id="a9def-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a9def-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9def-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="a9def-112">vppTokenId</span></span>|<span data-ttu-id="a9def-113">String</span><span class="sxs-lookup"><span data-stu-id="a9def-113">String</span></span>|<span data-ttu-id="a9def-114">Bezeichner des Tokens VPP.</span><span class="sxs-lookup"><span data-stu-id="a9def-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="a9def-115">appleId</span><span class="sxs-lookup"><span data-stu-id="a9def-115">appleId</span></span>|<span data-ttu-id="a9def-116">String</span><span class="sxs-lookup"><span data-stu-id="a9def-116">String</span></span>|<span data-ttu-id="a9def-117">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="a9def-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a9def-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="a9def-118">organizationName</span></span>|<span data-ttu-id="a9def-119">String</span><span class="sxs-lookup"><span data-stu-id="a9def-119">String</span></span>|<span data-ttu-id="a9def-120">Die Organisation Apple Volume Purchase Programm Token zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="a9def-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="a9def-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a9def-121">availableLicenseCount</span></span>|<span data-ttu-id="a9def-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a9def-122">Int32</span></span>|<span data-ttu-id="a9def-123">Die Anzahl der VPP Lizenzen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="a9def-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="a9def-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a9def-124">usedLicenseCount</span></span>|<span data-ttu-id="a9def-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a9def-125">Int32</span></span>|<span data-ttu-id="a9def-126">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="a9def-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9def-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a9def-127">Relationships</span></span>
<span data-ttu-id="a9def-128">Keine</span><span class="sxs-lookup"><span data-stu-id="a9def-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a9def-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a9def-129">JSON Representation</span></span>
<span data-ttu-id="a9def-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a9def-130">Here is a JSON representation of the resource.</span></span>
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





