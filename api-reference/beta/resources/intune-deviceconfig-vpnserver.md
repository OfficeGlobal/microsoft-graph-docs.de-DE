---
title: vpnServer-Ressourcentyp
description: VPN-Server Definition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9dd09e7ab0280120dd207424a862696ba087e20c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170462"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="b6473-103">vpnServer-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b6473-103">vpnServer resource type</span></span>

> <span data-ttu-id="b6473-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6473-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6473-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b6473-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6473-106">VPN-Server Definition.</span><span class="sxs-lookup"><span data-stu-id="b6473-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b6473-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b6473-107">Properties</span></span>
|<span data-ttu-id="b6473-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b6473-108">Property</span></span>|<span data-ttu-id="b6473-109">Typ</span><span class="sxs-lookup"><span data-stu-id="b6473-109">Type</span></span>|<span data-ttu-id="b6473-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b6473-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6473-111">description</span><span class="sxs-lookup"><span data-stu-id="b6473-111">description</span></span>|<span data-ttu-id="b6473-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b6473-112">String</span></span>|<span data-ttu-id="b6473-113">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="b6473-113">Description.</span></span>|
|<span data-ttu-id="b6473-114">address</span><span class="sxs-lookup"><span data-stu-id="b6473-114">address</span></span>|<span data-ttu-id="b6473-115">String</span><span class="sxs-lookup"><span data-stu-id="b6473-115">String</span></span>|<span data-ttu-id="b6473-116">Adresse (IP-Adresse, FQDN oder URL)</span><span class="sxs-lookup"><span data-stu-id="b6473-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="b6473-117">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="b6473-117">isDefaultServer</span></span>|<span data-ttu-id="b6473-118">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b6473-118">Boolean</span></span>|<span data-ttu-id="b6473-119">Standardserver.</span><span class="sxs-lookup"><span data-stu-id="b6473-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6473-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b6473-120">Relationships</span></span>
<span data-ttu-id="b6473-121">Keine</span><span class="sxs-lookup"><span data-stu-id="b6473-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6473-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b6473-122">JSON Representation</span></span>
<span data-ttu-id="b6473-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b6473-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```




