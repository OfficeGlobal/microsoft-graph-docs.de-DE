---
title: omaSetting-Ressourcentyp
description: Definition der OMA-Einstellungen.
ms.openlocfilehash: 900e3f4d8e24743ed75b15f7a57188b46630c9fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059401"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="d5da4-103">omaSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d5da4-103">omaSetting resource type</span></span>

> <span data-ttu-id="d5da4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d5da4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5da4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d5da4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5da4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d5da4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5da4-107">Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="d5da4-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="d5da4-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d5da4-108">Properties</span></span>
|<span data-ttu-id="d5da4-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d5da4-109">Property</span></span>|<span data-ttu-id="d5da4-110">Typ</span><span class="sxs-lookup"><span data-stu-id="d5da4-110">Type</span></span>|<span data-ttu-id="d5da4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5da4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5da4-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d5da4-112">displayName</span></span>|<span data-ttu-id="d5da4-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d5da4-113">String</span></span>|<span data-ttu-id="d5da4-114">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="d5da4-114">Display Name.</span></span>|
|<span data-ttu-id="d5da4-115">description</span><span class="sxs-lookup"><span data-stu-id="d5da4-115">description</span></span>|<span data-ttu-id="d5da4-116">String</span><span class="sxs-lookup"><span data-stu-id="d5da4-116">String</span></span>|<span data-ttu-id="d5da4-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="d5da4-117">Description.</span></span>|
|<span data-ttu-id="d5da4-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="d5da4-118">omaUri</span></span>|<span data-ttu-id="d5da4-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d5da4-119">String</span></span>|<span data-ttu-id="d5da4-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="d5da4-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5da4-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d5da4-121">Relationships</span></span>
<span data-ttu-id="d5da4-122">Keine</span><span class="sxs-lookup"><span data-stu-id="d5da4-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d5da4-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d5da4-123">JSON Representation</span></span>
<span data-ttu-id="d5da4-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d5da4-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```





