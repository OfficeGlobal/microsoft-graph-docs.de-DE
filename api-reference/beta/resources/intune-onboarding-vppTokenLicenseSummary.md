---
title: Ressourcentyp vppTokenLicenseSummary
description: Lizenz-Zusammenfassung der eine bestimmte app in einem Token.
ms.openlocfilehash: fba888c706b21a796615bf9bc2ea79968d5ad6d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059798"
---
# <a name="vpptokenlicensesummary-resource-type"></a><span data-ttu-id="ff4cf-103">Ressourcentyp vppTokenLicenseSummary</span><span class="sxs-lookup"><span data-stu-id="ff4cf-103">vppTokenLicenseSummary resource type</span></span>

> <span data-ttu-id="ff4cf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff4cf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff4cf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff4cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff4cf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff4cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff4cf-107">Lizenz-Zusammenfassung der eine bestimmte app in einem Token.</span><span class="sxs-lookup"><span data-stu-id="ff4cf-107">License summary of a given app in a token.</span></span>
## <a name="properties"></a><span data-ttu-id="ff4cf-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ff4cf-108">Properties</span></span>
|<span data-ttu-id="ff4cf-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff4cf-109">Property</span></span>|<span data-ttu-id="ff4cf-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ff4cf-110">Type</span></span>|<span data-ttu-id="ff4cf-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff4cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff4cf-112">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="ff4cf-112">vppTokenId</span></span>|<span data-ttu-id="ff4cf-113">String</span><span class="sxs-lookup"><span data-stu-id="ff4cf-113">String</span></span>|<span data-ttu-id="ff4cf-114">Bezeichner des Tokens VPP.</span><span class="sxs-lookup"><span data-stu-id="ff4cf-114">Identifier of the VPP token.</span></span>|
|<span data-ttu-id="ff4cf-115">appleId</span><span class="sxs-lookup"><span data-stu-id="ff4cf-115">appleId</span></span>|<span data-ttu-id="ff4cf-116">String</span><span class="sxs-lookup"><span data-stu-id="ff4cf-116">String</span></span>|<span data-ttu-id="ff4cf-117">Apple-ID, die dem Apple Volume Purchase Program-Token zugeordnet ist</span><span class="sxs-lookup"><span data-stu-id="ff4cf-117">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ff4cf-118">organizationName</span><span class="sxs-lookup"><span data-stu-id="ff4cf-118">organizationName</span></span>|<span data-ttu-id="ff4cf-119">String</span><span class="sxs-lookup"><span data-stu-id="ff4cf-119">String</span></span>|<span data-ttu-id="ff4cf-120">Die Organisation Apple Volume Purchase Programm Token zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="ff4cf-120">The organization associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ff4cf-121">availableLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ff4cf-121">availableLicenseCount</span></span>|<span data-ttu-id="ff4cf-122">Int32</span><span class="sxs-lookup"><span data-stu-id="ff4cf-122">Int32</span></span>|<span data-ttu-id="ff4cf-123">Die Anzahl der VPP Lizenzen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="ff4cf-123">The number of VPP licenses available.</span></span>|
|<span data-ttu-id="ff4cf-124">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ff4cf-124">usedLicenseCount</span></span>|<span data-ttu-id="ff4cf-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ff4cf-125">Int32</span></span>|<span data-ttu-id="ff4cf-126">Anzahl von VPP-Lizenzen, die aktuell verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="ff4cf-126">The number of VPP licenses in use.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff4cf-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ff4cf-127">Relationships</span></span>
<span data-ttu-id="ff4cf-128">Keine</span><span class="sxs-lookup"><span data-stu-id="ff4cf-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff4cf-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ff4cf-129">JSON Representation</span></span>
<span data-ttu-id="ff4cf-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ff4cf-130">Here is a JSON representation of the resource.</span></span>
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





