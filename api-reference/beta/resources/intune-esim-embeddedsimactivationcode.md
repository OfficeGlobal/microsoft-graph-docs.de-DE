---
title: Ressourcentyp embeddedSIMActivationCode
description: Der eingebettete SIM Aktivierungscode bereitgestellt vom Mobilfunkbetreiber.
author: tfitzmac
ms.openlocfilehash: 4e768a4047b8ddc785b545d3b850128a8e44f256
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311788"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="aadff-103">Ressourcentyp embeddedSIMActivationCode</span><span class="sxs-lookup"><span data-stu-id="aadff-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="aadff-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aadff-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aadff-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aadff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aadff-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aadff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aadff-107">Der eingebettete SIM Aktivierungscode bereitgestellt vom Mobilfunkbetreiber.</span><span class="sxs-lookup"><span data-stu-id="aadff-107">The embedded SIM activation code as provided by the mobile operator.</span></span>
## <a name="properties"></a><span data-ttu-id="aadff-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="aadff-108">Properties</span></span>
|<span data-ttu-id="aadff-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="aadff-109">Property</span></span>|<span data-ttu-id="aadff-110">Typ</span><span class="sxs-lookup"><span data-stu-id="aadff-110">Type</span></span>|<span data-ttu-id="aadff-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aadff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aadff-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="aadff-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="aadff-113">String</span><span class="sxs-lookup"><span data-stu-id="aadff-113">String</span></span>|<span data-ttu-id="aadff-114">Chip Karte Bezeichner (ICCID) für diesen eingebettet SIM Aktivierungscode vom Mobilfunkbetreiber bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="aadff-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="aadff-115">Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^\[0-9\]{19}\[0-9\]?$ '.</span><span class="sxs-lookup"><span data-stu-id="aadff-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="aadff-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="aadff-116">matchingIdentifier</span></span>|<span data-ttu-id="aadff-117">String</span><span class="sxs-lookup"><span data-stu-id="aadff-117">String</span></span>|<span data-ttu-id="aadff-118">Die MatchingIdentifier (MatchingID) gemäß den GSMA Zuordnung SGP.22 RSP technischen Spezifikationen Abschnitt 4.1.</span><span class="sxs-lookup"><span data-stu-id="aadff-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="aadff-119">Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^\[a-zA-Z0-9\-\]\* $'.</span><span class="sxs-lookup"><span data-stu-id="aadff-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="aadff-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="aadff-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="aadff-121">String</span><span class="sxs-lookup"><span data-stu-id="aadff-121">String</span></span>|<span data-ttu-id="aadff-122">Der vollqualifizierte Domänenname des des SM-DP + Server wie in der technischen g/m2 Zuordnung SPG.22 RSP-Spezifikation angegeben.</span><span class="sxs-lookup"><span data-stu-id="aadff-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="aadff-123">Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) \*\.) +\[a-zA-Z\]{2,}$'.</span><span class="sxs-lookup"><span data-stu-id="aadff-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aadff-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="aadff-124">Relationships</span></span>
<span data-ttu-id="aadff-125">Keine</span><span class="sxs-lookup"><span data-stu-id="aadff-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aadff-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="aadff-126">JSON Representation</span></span>
<span data-ttu-id="aadff-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="aadff-127">Here is a JSON representation of the resource.</span></span>
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





