---
title: proxiedDomain-Ressourcentyp
description: Beschreibt die ProxiedDomain Ressource die Microsoft Graph-API für Intune, die mehrere Workflows unterstützt.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b13e880508c80a009eacb520452c66e7b733ad86
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421844"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="eafc3-103">proxiedDomain-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="eafc3-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="eafc3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eafc3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eafc3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eafc3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eafc3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eafc3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eafc3-107">Proxydomäne</span><span class="sxs-lookup"><span data-stu-id="eafc3-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="eafc3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eafc3-108">Properties</span></span>
|<span data-ttu-id="eafc3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eafc3-109">Property</span></span>|<span data-ttu-id="eafc3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="eafc3-110">Type</span></span>|<span data-ttu-id="eafc3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eafc3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eafc3-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="eafc3-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="eafc3-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eafc3-113">String</span></span>|<span data-ttu-id="eafc3-114">Die IP-Adresse oder vollqualifizierten Domänennamen (FQDN).</span><span class="sxs-lookup"><span data-stu-id="eafc3-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="eafc3-115">Proxy</span><span class="sxs-lookup"><span data-stu-id="eafc3-115">proxy</span></span>|<span data-ttu-id="eafc3-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eafc3-116">String</span></span>|<span data-ttu-id="eafc3-117">Proxy-IP-Adresse oder FQDN.</span><span class="sxs-lookup"><span data-stu-id="eafc3-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eafc3-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="eafc3-118">Relationships</span></span>
<span data-ttu-id="eafc3-119">Keine</span><span class="sxs-lookup"><span data-stu-id="eafc3-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eafc3-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eafc3-120">JSON Representation</span></span>
<span data-ttu-id="eafc3-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eafc3-121">Here is a JSON representation of the resource.</span></span>
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



