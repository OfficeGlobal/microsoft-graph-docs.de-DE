---
title: omaSetting-Ressourcentyp
description: Definition der OMA-Einstellungen.
author: tfitzmac
ms.openlocfilehash: fa1fc438ef97357ebd5f13443077384bc98e24f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314042"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="6372e-103">omaSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6372e-103">omaSetting resource type</span></span>

> <span data-ttu-id="6372e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6372e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6372e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6372e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6372e-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6372e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6372e-107">Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="6372e-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="6372e-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6372e-108">Properties</span></span>
|<span data-ttu-id="6372e-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6372e-109">Property</span></span>|<span data-ttu-id="6372e-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6372e-110">Type</span></span>|<span data-ttu-id="6372e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6372e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6372e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6372e-112">displayName</span></span>|<span data-ttu-id="6372e-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6372e-113">String</span></span>|<span data-ttu-id="6372e-114">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="6372e-114">Display Name.</span></span>|
|<span data-ttu-id="6372e-115">description</span><span class="sxs-lookup"><span data-stu-id="6372e-115">description</span></span>|<span data-ttu-id="6372e-116">String</span><span class="sxs-lookup"><span data-stu-id="6372e-116">String</span></span>|<span data-ttu-id="6372e-117">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="6372e-117">Description.</span></span>|
|<span data-ttu-id="6372e-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="6372e-118">omaUri</span></span>|<span data-ttu-id="6372e-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6372e-119">String</span></span>|<span data-ttu-id="6372e-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="6372e-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6372e-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6372e-121">Relationships</span></span>
<span data-ttu-id="6372e-122">Keine</span><span class="sxs-lookup"><span data-stu-id="6372e-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6372e-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6372e-123">JSON Representation</span></span>
<span data-ttu-id="6372e-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6372e-124">Here is a JSON representation of the resource.</span></span>
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





