---
title: VpnServer Ressourcentyp
description: VPN-Server-Definition.
ms.openlocfilehash: e89cc562c3fe0f6b353199ca7de639053177ab1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061600"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="595a7-103">VpnServer Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="595a7-103">vpnServer resource type</span></span>

> <span data-ttu-id="595a7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="595a7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="595a7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="595a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="595a7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="595a7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="595a7-107">VPN-Server-Definition.</span><span class="sxs-lookup"><span data-stu-id="595a7-107">VPN Server definition.</span></span>
## <a name="properties"></a><span data-ttu-id="595a7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="595a7-108">Properties</span></span>
|<span data-ttu-id="595a7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="595a7-109">Property</span></span>|<span data-ttu-id="595a7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="595a7-110">Type</span></span>|<span data-ttu-id="595a7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="595a7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="595a7-112">description</span><span class="sxs-lookup"><span data-stu-id="595a7-112">description</span></span>|<span data-ttu-id="595a7-113">String</span><span class="sxs-lookup"><span data-stu-id="595a7-113">String</span></span>|<span data-ttu-id="595a7-114">Beschreibung.</span><span class="sxs-lookup"><span data-stu-id="595a7-114">Description.</span></span>|
|<span data-ttu-id="595a7-115">address</span><span class="sxs-lookup"><span data-stu-id="595a7-115">address</span></span>|<span data-ttu-id="595a7-116">String</span><span class="sxs-lookup"><span data-stu-id="595a7-116">String</span></span>|<span data-ttu-id="595a7-117">(IP-Adresse, FQDN oder die URL)</span><span class="sxs-lookup"><span data-stu-id="595a7-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="595a7-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="595a7-118">isDefaultServer</span></span>|<span data-ttu-id="595a7-119">Boolesch</span><span class="sxs-lookup"><span data-stu-id="595a7-119">Boolean</span></span>|<span data-ttu-id="595a7-120">Standardserver.</span><span class="sxs-lookup"><span data-stu-id="595a7-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="595a7-121">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="595a7-121">Relationships</span></span>
<span data-ttu-id="595a7-122">Keine</span><span class="sxs-lookup"><span data-stu-id="595a7-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="595a7-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="595a7-123">JSON Representation</span></span>
<span data-ttu-id="595a7-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="595a7-124">Here is a JSON representation of the resource.</span></span>
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





