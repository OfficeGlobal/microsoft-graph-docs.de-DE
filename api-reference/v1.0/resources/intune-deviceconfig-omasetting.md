---
title: omaSetting-Ressourcentyp
description: Definition der OMA-Einstellungen.
author: tfitzmac
ms.openlocfilehash: 564912635fbcd5e2846965d3546a3830119db252
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340887"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="caca0-103">omaSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="caca0-103">omaSetting resource type</span></span>

> <span data-ttu-id="caca0-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="caca0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="caca0-105">Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="caca0-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="caca0-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="caca0-106">Properties</span></span>
|<span data-ttu-id="caca0-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="caca0-107">Property</span></span>|<span data-ttu-id="caca0-108">Typ</span><span class="sxs-lookup"><span data-stu-id="caca0-108">Type</span></span>|<span data-ttu-id="caca0-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="caca0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caca0-110">displayName</span><span class="sxs-lookup"><span data-stu-id="caca0-110">displayName</span></span>|<span data-ttu-id="caca0-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="caca0-111">String</span></span>|<span data-ttu-id="caca0-112">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="caca0-112">Display Name.</span></span>|
|<span data-ttu-id="caca0-113">description</span><span class="sxs-lookup"><span data-stu-id="caca0-113">description</span></span>|<span data-ttu-id="caca0-114">String</span><span class="sxs-lookup"><span data-stu-id="caca0-114">String</span></span>|<span data-ttu-id="caca0-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="caca0-115">Description.</span></span>|
|<span data-ttu-id="caca0-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="caca0-116">omaUri</span></span>|<span data-ttu-id="caca0-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="caca0-117">String</span></span>|<span data-ttu-id="caca0-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="caca0-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="caca0-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="caca0-119">Relationships</span></span>
<span data-ttu-id="caca0-120">Keine</span><span class="sxs-lookup"><span data-stu-id="caca0-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="caca0-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="caca0-121">JSON Representation</span></span>
<span data-ttu-id="caca0-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="caca0-122">Here is a JSON representation of the resource.</span></span>
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



