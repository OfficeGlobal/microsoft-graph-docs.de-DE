---
title: omaSetting-Ressourcentyp
description: Definition der OMA-Einstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 42b6d5fcea7b3b46acf8d0a119213f679d99aed6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961484"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="13223-103">omaSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="13223-103">omaSetting resource type</span></span>

> <span data-ttu-id="13223-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="13223-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13223-105">Definition der OMA-Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="13223-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="13223-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="13223-106">Properties</span></span>
|<span data-ttu-id="13223-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="13223-107">Property</span></span>|<span data-ttu-id="13223-108">Typ</span><span class="sxs-lookup"><span data-stu-id="13223-108">Type</span></span>|<span data-ttu-id="13223-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="13223-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13223-110">displayName</span><span class="sxs-lookup"><span data-stu-id="13223-110">displayName</span></span>|<span data-ttu-id="13223-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13223-111">String</span></span>|<span data-ttu-id="13223-112">Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="13223-112">Display Name.</span></span>|
|<span data-ttu-id="13223-113">description</span><span class="sxs-lookup"><span data-stu-id="13223-113">description</span></span>|<span data-ttu-id="13223-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13223-114">String</span></span>|<span data-ttu-id="13223-115">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="13223-115">Description.</span></span>|
|<span data-ttu-id="13223-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="13223-116">omaUri</span></span>|<span data-ttu-id="13223-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="13223-117">String</span></span>|<span data-ttu-id="13223-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="13223-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13223-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="13223-119">Relationships</span></span>
<span data-ttu-id="13223-120">Keine</span><span class="sxs-lookup"><span data-stu-id="13223-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13223-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="13223-121">JSON Representation</span></span>
<span data-ttu-id="13223-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="13223-122">Here is a JSON representation of the resource.</span></span>
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



