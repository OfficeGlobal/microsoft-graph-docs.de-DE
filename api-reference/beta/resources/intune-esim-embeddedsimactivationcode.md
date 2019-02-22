---
title: embeddedSIMActivationCode-Ressourcentyp
description: Der eingebettete SIM-Aktivierungscode, der vom Mobilfunkanbieter bereitgestellt wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 955dccb226332b297e30c4d40768f84936b04dbe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145227"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="d70a3-103">embeddedSIMActivationCode-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d70a3-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="d70a3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d70a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d70a3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d70a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d70a3-106">Der eingebettete SIM-Aktivierungscode, der vom Mobilfunkanbieter bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="d70a3-106">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="d70a3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d70a3-107">Properties</span></span>
|<span data-ttu-id="d70a3-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d70a3-108">Property</span></span>|<span data-ttu-id="d70a3-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d70a3-109">Type</span></span>|<span data-ttu-id="d70a3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d70a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d70a3-111">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="d70a3-111">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="d70a3-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d70a3-112">String</span></span>|<span data-ttu-id="d70a3-113">Der integrierte Leiterkarten Bezeichner (ICCID) für diesen eingebetteten SIM-Aktivierungscode, der vom Mobilfunkanbieter bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="d70a3-113">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="d70a3-114">die eingabe muss mit dem folgenden regulären ausdruck übereinstimmen:\['\]{19}\[^\]0-9 0-9 ? $ '.</span><span class="sxs-lookup"><span data-stu-id="d70a3-114">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="d70a3-115">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="d70a3-115">matchingIdentifier</span></span>|<span data-ttu-id="d70a3-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d70a3-116">String</span></span>|<span data-ttu-id="d70a3-117">Die MatchingIdentifier (übereinstimmende) gemäß der GSMA Association SGP. 22 RSP Technical Specification section 4,1.</span><span class="sxs-lookup"><span data-stu-id="d70a3-117">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="d70a3-118">Die Eingabe muss mit dem folgenden regulären Ausdruck übereinstimmen:\[' ^ a-zA-Z0\-\]-9 \* $ '.</span><span class="sxs-lookup"><span data-stu-id="d70a3-118">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="d70a3-119">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="d70a3-119">smdpPlusServerAddress</span></span>|<span data-ttu-id="d70a3-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d70a3-120">String</span></span>|<span data-ttu-id="d70a3-121">Der vollqualifizierte Domänenname des SM-DP +-Servers gemäß der technischen Spezifikation des GSM-Verbandes SPG .22 RSP.</span><span class="sxs-lookup"><span data-stu-id="d70a3-121">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="d70a3-122">Die Eingabe muss mit dem folgenden regulären Ausdruck übereinstimmen: '\[^ (a-zA-Z0\]-9 +\[(-a-zA-Z0\]-9 +\.) \*\[) + a-za\]{2,}-Z $ '.</span><span class="sxs-lookup"><span data-stu-id="d70a3-122">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d70a3-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d70a3-123">Relationships</span></span>
<span data-ttu-id="d70a3-124">Keine</span><span class="sxs-lookup"><span data-stu-id="d70a3-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d70a3-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d70a3-125">JSON Representation</span></span>
<span data-ttu-id="d70a3-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d70a3-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCode",
  "integratedCircuitCardIdentifier": "String",
  "matchingIdentifier": "String",
  "smdpPlusServerAddress": "String"
}
```




