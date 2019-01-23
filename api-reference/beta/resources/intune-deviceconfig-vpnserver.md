---
title: VpnServer Ressourcentyp
description: VPN-Server-Definition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0febdae5745f1295e9c690213d4a51b79d7d3bdb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406808"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="71873-103">VpnServer Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="71873-103">vpnServer resource type</span></span>

> <span data-ttu-id="71873-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="71873-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="71873-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="71873-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="71873-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="71873-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71873-107">VPN-Server-Definition.</span><span class="sxs-lookup"><span data-stu-id="71873-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="71873-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="71873-108">Properties</span></span>
|<span data-ttu-id="71873-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="71873-109">Property</span></span>|<span data-ttu-id="71873-110">Typ</span><span class="sxs-lookup"><span data-stu-id="71873-110">Type</span></span>|<span data-ttu-id="71873-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="71873-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71873-112">description</span><span class="sxs-lookup"><span data-stu-id="71873-112">description</span></span>|<span data-ttu-id="71873-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="71873-113">String</span></span>|<span data-ttu-id="71873-114">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="71873-114">Description.</span></span>|
|<span data-ttu-id="71873-115">address</span><span class="sxs-lookup"><span data-stu-id="71873-115">address</span></span>|<span data-ttu-id="71873-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="71873-116">String</span></span>|<span data-ttu-id="71873-117">(IP-Adresse, FQDN oder die URL)</span><span class="sxs-lookup"><span data-stu-id="71873-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="71873-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="71873-118">isDefaultServer</span></span>|<span data-ttu-id="71873-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="71873-119">Boolean</span></span>|<span data-ttu-id="71873-120">Standardserver.</span><span class="sxs-lookup"><span data-stu-id="71873-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71873-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="71873-121">Relationships</span></span>
<span data-ttu-id="71873-122">Keine</span><span class="sxs-lookup"><span data-stu-id="71873-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71873-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="71873-123">JSON Representation</span></span>
<span data-ttu-id="71873-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="71873-124">Here is a JSON representation of the resource.</span></span>
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




