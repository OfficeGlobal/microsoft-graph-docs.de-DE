---
title: omaSetting-Ressourcentyp
description: Definition der OMA-Einstellungen.
ms.openlocfilehash: 7ef8617ca4ce10ebeabf0d7a4655688e58925646
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017402"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="9c22b-103">omaSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9c22b-103">omaSetting resource type</span></span>

> <span data-ttu-id="9c22b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9c22b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c22b-105">Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="9c22b-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="9c22b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9c22b-106">Properties</span></span>
|<span data-ttu-id="9c22b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9c22b-107">Property</span></span>|<span data-ttu-id="9c22b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="9c22b-108">Type</span></span>|<span data-ttu-id="9c22b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9c22b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c22b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9c22b-110">displayName</span></span>|<span data-ttu-id="9c22b-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9c22b-111">String</span></span>|<span data-ttu-id="9c22b-112">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="9c22b-112">Display Name.</span></span>|
|<span data-ttu-id="9c22b-113">description</span><span class="sxs-lookup"><span data-stu-id="9c22b-113">description</span></span>|<span data-ttu-id="9c22b-114">String</span><span class="sxs-lookup"><span data-stu-id="9c22b-114">String</span></span>|<span data-ttu-id="9c22b-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="9c22b-115">Description.</span></span>|
|<span data-ttu-id="9c22b-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="9c22b-116">omaUri</span></span>|<span data-ttu-id="9c22b-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9c22b-117">String</span></span>|<span data-ttu-id="9c22b-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="9c22b-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c22b-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9c22b-119">Relationships</span></span>
<span data-ttu-id="9c22b-120">Keine</span><span class="sxs-lookup"><span data-stu-id="9c22b-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9c22b-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9c22b-121">JSON Representation</span></span>
<span data-ttu-id="9c22b-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9c22b-122">Here is a JSON representation of the resource.</span></span>
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



