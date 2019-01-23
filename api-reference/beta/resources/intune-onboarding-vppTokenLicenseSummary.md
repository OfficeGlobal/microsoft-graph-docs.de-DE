---
title: Ressourcentyp vppTokenLicenseSummary
description: Lizenz-Zusammenfassung der eine bestimmte app in einem Token.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8fb84a549d95459db1e4b39c11b526f73db08752
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395181"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="089f2-103">Ressourcentyp vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="089f2-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="089f2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="089f2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="089f2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="089f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="089f2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="089f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="089f2-107">Lizenz-Zusammenfassung der eine bestimmte app in einem Token.</span><span class="sxs-lookup"><span data-stu-id="089f2-107">License summary of a given app in a token.</span></span>

## <a name="properties"></a><span data-ttu-id="089f2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="089f2-108">Properties</span></span>
|<span data-ttu-id="089f2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="089f2-109">Property</span></span>|<span data-ttu-id="089f2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="089f2-110">Type</span></span>|<span data-ttu-id="089f2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="089f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="089f2-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="089f2-112">vppTokenId</span></span>|<span data-ttu-id="089f2-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="089f2-113">String</span></span>|<span data-ttu-id="089f2-114">Bezeichner des Tokens VPP.</span><span class="sxs-lookup"><span data-stu-id="089f2-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="089f2-115">appleId</span><span class="sxs-lookup"><span data-stu-id="089f2-115">appleId</span></span>|<span data-ttu-id="089f2-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="089f2-116">String</span></span>|<span data-ttu-id="089f2-117">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="089f2-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="089f2-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="089f2-118">organizationName</span></span>|<span data-ttu-id="089f2-119">String</span><span class="sxs-lookup"><span data-stu-id="089f2-119">String</span></span>|<span data-ttu-id="089f2-120">Die Organisation Apple Volume Purchase Programm Token zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="089f2-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="089f2-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="089f2-121">availableLicenseCount</span></span>|<span data-ttu-id="089f2-122">Int32</span><span class="sxs-lookup"><span data-stu-id="089f2-122">Int32</span></span>|<span data-ttu-id="089f2-123">Die Anzahl der VPP Lizenzen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="089f2-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="089f2-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="089f2-124">usedLicenseCount</span></span>|<span data-ttu-id="089f2-125">Int32</span><span class="sxs-lookup"><span data-stu-id="089f2-125">Int32</span></span>|<span data-ttu-id="089f2-126">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="089f2-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="089f2-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="089f2-127">Relationships</span></span>
<span data-ttu-id="089f2-128">Keine</span><span class="sxs-lookup"><span data-stu-id="089f2-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="089f2-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="089f2-129">JSON Representation</span></span>
<span data-ttu-id="089f2-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="089f2-130">Here is a JSON representation of the resource.</span></span>
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




