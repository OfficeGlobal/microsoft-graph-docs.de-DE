---
title: proxiedDomain-Ressourcentyp
description: Proxydomäne
ms.openlocfilehash: 310ccb1420ed450c9e7c53d534181720f9051ff4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059177"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="6ecdf-103">proxiedDomain-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="6ecdf-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="6ecdf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6ecdf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ecdf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6ecdf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ecdf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6ecdf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ecdf-107">Proxydomäne</span><span class="sxs-lookup"><span data-stu-id="6ecdf-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="6ecdf-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6ecdf-108">Properties</span></span>
|<span data-ttu-id="6ecdf-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6ecdf-109">Property</span></span>|<span data-ttu-id="6ecdf-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6ecdf-110">Type</span></span>|<span data-ttu-id="6ecdf-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6ecdf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ecdf-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="6ecdf-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="6ecdf-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ecdf-113">String</span></span>|<span data-ttu-id="6ecdf-114">Die IP-Adresse oder vollqualifizierten Domänennamen (FQDN).</span><span class="sxs-lookup"><span data-stu-id="6ecdf-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="6ecdf-115">Proxy</span><span class="sxs-lookup"><span data-stu-id="6ecdf-115">proxy</span></span>|<span data-ttu-id="6ecdf-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6ecdf-116">String</span></span>|<span data-ttu-id="6ecdf-117">Proxy-IP-Adresse oder FQDN.</span><span class="sxs-lookup"><span data-stu-id="6ecdf-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ecdf-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6ecdf-118">Relationships</span></span>
<span data-ttu-id="6ecdf-119">Keine</span><span class="sxs-lookup"><span data-stu-id="6ecdf-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ecdf-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6ecdf-120">JSON Representation</span></span>
<span data-ttu-id="6ecdf-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6ecdf-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



