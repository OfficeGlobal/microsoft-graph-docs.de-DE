---
title: Ressourcentyp embeddedSIMActivationCode
description: Der eingebettete SIM Aktivierungscode bereitgestellt vom Mobilfunkbetreiber.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: af8bf020953dbc014f42aa6d363d3ca9e30db8a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987405"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="173ed-103">Ressourcentyp embeddedSIMActivationCode</span><span class="sxs-lookup"><span data-stu-id="173ed-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="173ed-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="173ed-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="173ed-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="173ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="173ed-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="173ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="173ed-107">Der eingebettete SIM Aktivierungscode bereitgestellt vom Mobilfunkbetreiber.</span><span class="sxs-lookup"><span data-stu-id="173ed-107">The embedded SIM activation code as provided by the mobile operator.</span></span>
## <a name="properties"></a><span data-ttu-id="173ed-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="173ed-108">Properties</span></span>
|<span data-ttu-id="173ed-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="173ed-109">Property</span></span>|<span data-ttu-id="173ed-110">Typ</span><span class="sxs-lookup"><span data-stu-id="173ed-110">Type</span></span>|<span data-ttu-id="173ed-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="173ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="173ed-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="173ed-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="173ed-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="173ed-113">String</span></span>|<span data-ttu-id="173ed-114">Chip Karte Bezeichner (ICCID) für diesen eingebettet SIM Aktivierungscode vom Mobilfunkbetreiber bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="173ed-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="173ed-115">Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^\[0-9\]{19}\[0-9\]?$ '.</span><span class="sxs-lookup"><span data-stu-id="173ed-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="173ed-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="173ed-116">matchingIdentifier</span></span>|<span data-ttu-id="173ed-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="173ed-117">String</span></span>|<span data-ttu-id="173ed-118">Die MatchingIdentifier (MatchingID) gemäß den GSMA Zuordnung SGP.22 RSP technischen Spezifikationen Abschnitt 4.1.</span><span class="sxs-lookup"><span data-stu-id="173ed-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="173ed-119">Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^\[a-zA-Z0-9\-\]\* $'.</span><span class="sxs-lookup"><span data-stu-id="173ed-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="173ed-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="173ed-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="173ed-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="173ed-121">String</span></span>|<span data-ttu-id="173ed-122">Der vollqualifizierte Domänenname des des SM-DP + Server wie in der technischen g/m2 Zuordnung SPG.22 RSP-Spezifikation angegeben.</span><span class="sxs-lookup"><span data-stu-id="173ed-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="173ed-123">Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) \*\.) +\[a-zA-Z\]{2,}$'.</span><span class="sxs-lookup"><span data-stu-id="173ed-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="173ed-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="173ed-124">Relationships</span></span>
<span data-ttu-id="173ed-125">Keine</span><span class="sxs-lookup"><span data-stu-id="173ed-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="173ed-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="173ed-126">JSON Representation</span></span>
<span data-ttu-id="173ed-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="173ed-127">Here is a JSON representation of the resource.</span></span>
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





