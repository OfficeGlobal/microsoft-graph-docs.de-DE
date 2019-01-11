---
title: Ressourcentyp embeddedSIMActivationCode
description: Der eingebettete SIM Aktivierungscode bereitgestellt vom Mobilfunkbetreiber.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 41976b92cfe6b6f695631dbd6c0d928c6ae99271
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878064"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="8037e-103">Ressourcentyp embeddedSIMActivationCode</span><span class="sxs-lookup"><span data-stu-id="8037e-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="8037e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8037e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8037e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8037e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8037e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8037e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8037e-107">Der eingebettete SIM Aktivierungscode bereitgestellt vom Mobilfunkbetreiber.</span><span class="sxs-lookup"><span data-stu-id="8037e-107">The embedded SIM activation code as provided by the mobile operator.</span></span>
## <a name="properties"></a><span data-ttu-id="8037e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8037e-108">Properties</span></span>
|<span data-ttu-id="8037e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8037e-109">Property</span></span>|<span data-ttu-id="8037e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8037e-110">Type</span></span>|<span data-ttu-id="8037e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8037e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8037e-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="8037e-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="8037e-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8037e-113">String</span></span>|<span data-ttu-id="8037e-114">Chip Karte Bezeichner (ICCID) für diesen eingebettet SIM Aktivierungscode vom Mobilfunkbetreiber bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="8037e-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="8037e-115">Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^\[0-9\]{19}\[0-9\]?$ '.</span><span class="sxs-lookup"><span data-stu-id="8037e-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="8037e-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="8037e-116">matchingIdentifier</span></span>|<span data-ttu-id="8037e-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8037e-117">String</span></span>|<span data-ttu-id="8037e-118">Die MatchingIdentifier (MatchingID) gemäß den GSMA Zuordnung SGP.22 RSP technischen Spezifikationen Abschnitt 4.1.</span><span class="sxs-lookup"><span data-stu-id="8037e-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="8037e-119">Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^\[a-zA-Z0-9\-\]\* $'.</span><span class="sxs-lookup"><span data-stu-id="8037e-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="8037e-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="8037e-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="8037e-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8037e-121">String</span></span>|<span data-ttu-id="8037e-122">Der vollqualifizierte Domänenname des des SM-DP + Server wie in der technischen g/m2 Zuordnung SPG.22 RSP-Spezifikation angegeben.</span><span class="sxs-lookup"><span data-stu-id="8037e-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="8037e-123">Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) \*\.) +\[a-zA-Z\]{2,}$'.</span><span class="sxs-lookup"><span data-stu-id="8037e-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8037e-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8037e-124">Relationships</span></span>
<span data-ttu-id="8037e-125">Keine</span><span class="sxs-lookup"><span data-stu-id="8037e-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8037e-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8037e-126">JSON Representation</span></span>
<span data-ttu-id="8037e-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8037e-127">Here is a JSON representation of the resource.</span></span>
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





