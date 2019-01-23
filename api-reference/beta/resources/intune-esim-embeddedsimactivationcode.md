---
title: Ressourcentyp embeddedSIMActivationCode
description: Der eingebettete SIM Aktivierungscode bereitgestellt vom Mobilfunkbetreiber.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74f1725ab8f12cb103144dc1897e9bf965c5361b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422467"
---
# <a name="embeddedsimactivationcode-resource-type"></a><span data-ttu-id="ad305-103">Ressourcentyp embeddedSIMActivationCode</span><span class="sxs-lookup"><span data-stu-id="ad305-103">embeddedSIMActivationCode resource type</span></span>

> <span data-ttu-id="ad305-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ad305-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ad305-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ad305-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad305-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ad305-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad305-107">Der eingebettete SIM Aktivierungscode bereitgestellt vom Mobilfunkbetreiber.</span><span class="sxs-lookup"><span data-stu-id="ad305-107">The embedded SIM activation code as provided by the mobile operator.</span></span>

## <a name="properties"></a><span data-ttu-id="ad305-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ad305-108">Properties</span></span>
|<span data-ttu-id="ad305-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ad305-109">Property</span></span>|<span data-ttu-id="ad305-110">Typ</span><span class="sxs-lookup"><span data-stu-id="ad305-110">Type</span></span>|<span data-ttu-id="ad305-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ad305-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad305-112">integratedCircuitCardIdentifier</span><span class="sxs-lookup"><span data-stu-id="ad305-112">integratedCircuitCardIdentifier</span></span>|<span data-ttu-id="ad305-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ad305-113">String</span></span>|<span data-ttu-id="ad305-114">Chip Karte Bezeichner (ICCID) für diesen eingebettet SIM Aktivierungscode vom Mobilfunkbetreiber bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="ad305-114">The Integrated Circuit Card Identifier (ICCID) for this embedded SIM activation code as provided by the mobile operator.</span></span>
<span data-ttu-id="ad305-115">Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^\[0-9\]{19}\[0-9\]?$ '.</span><span class="sxs-lookup"><span data-stu-id="ad305-115">The input must match the following regular expression: '^\[0-9\]{19}\[0-9\]?$'.</span></span>|
|<span data-ttu-id="ad305-116">matchingIdentifier</span><span class="sxs-lookup"><span data-stu-id="ad305-116">matchingIdentifier</span></span>|<span data-ttu-id="ad305-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ad305-117">String</span></span>|<span data-ttu-id="ad305-118">Die MatchingIdentifier (MatchingID) gemäß den GSMA Zuordnung SGP.22 RSP technischen Spezifikationen Abschnitt 4.1.</span><span class="sxs-lookup"><span data-stu-id="ad305-118">The MatchingIdentifier (MatchingID) as specified in the GSMA Association SGP.22 RSP Technical Specification section 4.1.</span></span>
<span data-ttu-id="ad305-119">Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^\[a-zA-Z0-9\-\]\* $'.</span><span class="sxs-lookup"><span data-stu-id="ad305-119">The input must match the following regular expression: '^\[a-zA-Z0-9\-\]\*$'.</span></span>|
|<span data-ttu-id="ad305-120">smdpPlusServerAddress</span><span class="sxs-lookup"><span data-stu-id="ad305-120">smdpPlusServerAddress</span></span>|<span data-ttu-id="ad305-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ad305-121">String</span></span>|<span data-ttu-id="ad305-122">Der vollqualifizierte Domänenname des des SM-DP + Server wie in der technischen g/m2 Zuordnung SPG.22 RSP-Spezifikation angegeben.</span><span class="sxs-lookup"><span data-stu-id="ad305-122">The fully qualified domain name of the SM-DP+ server as specified in the GSM Association SPG .22 RSP Technical Specification.</span></span>
<span data-ttu-id="ad305-123">Die Eingabe muss den folgenden regulären Ausdruck übereinstimmen: ' ^ (\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+) \*\.) +\[a-zA-Z\]{2,}$'.</span><span class="sxs-lookup"><span data-stu-id="ad305-123">The input must match the following regular expression: '^(\[a-zA-Z0-9\]+(-\[a-zA-Z0-9\]+)\*\.)+\[a-zA-Z\]{2,}$'.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad305-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ad305-124">Relationships</span></span>
<span data-ttu-id="ad305-125">Keine</span><span class="sxs-lookup"><span data-stu-id="ad305-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad305-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ad305-126">JSON Representation</span></span>
<span data-ttu-id="ad305-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ad305-127">Here is a JSON representation of the resource.</span></span>
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




