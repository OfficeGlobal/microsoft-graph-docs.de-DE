---
title: Ressourcentyp conditionalAccessPolicy
description: Gibt an, dass die Attribute, die weiterführende eine bedingte Zugriffsrichtlinie oder Richtlinien, die von der entsprechenden Anmeldung Aktivität ausgelöst wird
localization_priority: Normal
ms.openlocfilehash: 7b043e739f84715fb02fbdbd25599e5cfccc284a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820643"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="57079-103">Ressourcentyp conditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="57079-103">conditionalAccessPolicy resource type</span></span>
<span data-ttu-id="57079-104">Gibt an, dass die Attribute, die weiterführende eine bedingte Zugriffsrichtlinie oder Richtlinien, die von der entsprechenden Anmeldung Aktivität ausgelöst wird</span><span class="sxs-lookup"><span data-stu-id="57079-104">Indicates the attributes related a conditional access policy or policies that's triggered by the corresponding sign-in activity</span></span>



## <a name="properties"></a><span data-ttu-id="57079-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="57079-105">Properties</span></span>
| <span data-ttu-id="57079-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="57079-106">Property</span></span>     | <span data-ttu-id="57079-107">Typ</span><span class="sxs-lookup"><span data-stu-id="57079-107">Type</span></span>   |<span data-ttu-id="57079-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="57079-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57079-109">displayName</span><span class="sxs-lookup"><span data-stu-id="57079-109">displayName</span></span>|<span data-ttu-id="57079-110">String</span><span class="sxs-lookup"><span data-stu-id="57079-110">String</span></span>|<span data-ttu-id="57079-111">Verweist auf den Namen der Richtlinie bedingten Zugriff (Beispiel: "Mehrstufiger Authentifizierung das für Vertriebs erfordern").</span><span class="sxs-lookup"><span data-stu-id="57079-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="57079-112">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="57079-112">enforcedGrantControls</span></span>|<span data-ttu-id="57079-113">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="57079-113">String collection</span></span>|<span data-ttu-id="57079-114">Bezieht sich auf die Grant-Steuerelemente, die durch die bedingte Zugriffsrichtlinie erzwungen (Beispiel: "Erfordern Multi-Factor Authentication").</span><span class="sxs-lookup"><span data-stu-id="57079-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="57079-115">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="57079-115">enforcedSessionControls</span></span>|<span data-ttu-id="57079-116">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="57079-116">String collection</span></span>|<span data-ttu-id="57079-117">Bezieht sich auf die Sitzung-Steuerelemente, die durch die bedingte Zugriffsrichtlinie erzwungen (Beispiel: "Erfordern app erzwungen Steuerelemente").</span><span class="sxs-lookup"><span data-stu-id="57079-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="57079-118">id</span><span class="sxs-lookup"><span data-stu-id="57079-118">id</span></span>|<span data-ttu-id="57079-119">String</span><span class="sxs-lookup"><span data-stu-id="57079-119">String</span></span>|<span data-ttu-id="57079-120">Eindeutige GUID bedingte-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="57079-120">Unique GUID of the conditional access policy</span></span>|
|<span data-ttu-id="57079-121">result</span><span class="sxs-lookup"><span data-stu-id="57079-121">result</span></span>|<span data-ttu-id="57079-122">String</span><span class="sxs-lookup"><span data-stu-id="57079-122">String</span></span>| <span data-ttu-id="57079-123">Gibt das Ergebnis der Zertifizierungsstellenrichtlinie, die ausgelöst wurde. Mögliche Werte sind:</span><span class="sxs-lookup"><span data-stu-id="57079-123">Indicates the result of the CA policy that was triggered.Possible values are:</span></span><br/> `success` <br/> `failure` <br/> <span data-ttu-id="57079-124">`notApplied`-Richtlinie wird nicht angewendet, da Drahtloszugriff nicht erfüllt wurden.</span><span class="sxs-lookup"><span data-stu-id="57079-124">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span> <br/> <span data-ttu-id="57079-125">`notEnabled`-Dies ist aufgrund der Richtlinie in deaktiviertem Zustand.</span><span class="sxs-lookup"><span data-stu-id="57079-125">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57079-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="57079-126">JSON representation</span></span>

<span data-ttu-id="57079-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="57079-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
