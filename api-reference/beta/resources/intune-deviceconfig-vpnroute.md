---
title: Ressourcentyp vpnRoute
description: VPN-Route Definition.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 628e2f384b06dece13da1595a4111a2d1022a673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423020"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="11eef-103">Ressourcentyp vpnRoute</span><span class="sxs-lookup"><span data-stu-id="11eef-103">vpnRoute resource type</span></span>

> <span data-ttu-id="11eef-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="11eef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="11eef-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="11eef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11eef-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="11eef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11eef-107">VPN-Route Definition.</span><span class="sxs-lookup"><span data-stu-id="11eef-107">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="11eef-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="11eef-108">Properties</span></span>
|<span data-ttu-id="11eef-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="11eef-109">Property</span></span>|<span data-ttu-id="11eef-110">Typ</span><span class="sxs-lookup"><span data-stu-id="11eef-110">Type</span></span>|<span data-ttu-id="11eef-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="11eef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11eef-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="11eef-112">destinationPrefix</span></span>|<span data-ttu-id="11eef-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="11eef-113">String</span></span>|<span data-ttu-id="11eef-114">Ziel-Präfix (/ v6 IPv4-Adresse).</span><span class="sxs-lookup"><span data-stu-id="11eef-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="11eef-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="11eef-115">prefixSize</span></span>|<span data-ttu-id="11eef-116">Int32</span><span class="sxs-lookup"><span data-stu-id="11eef-116">Int32</span></span>|<span data-ttu-id="11eef-117">Präfix Größe.</span><span class="sxs-lookup"><span data-stu-id="11eef-117">Prefix size.</span></span> <span data-ttu-id="11eef-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="11eef-118">(1-32).</span></span> <span data-ttu-id="11eef-119">Gültige Werte 1 bis 32</span><span class="sxs-lookup"><span data-stu-id="11eef-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="11eef-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="11eef-120">Relationships</span></span>
<span data-ttu-id="11eef-121">Keine</span><span class="sxs-lookup"><span data-stu-id="11eef-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11eef-122">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="11eef-122">JSON Representation</span></span>
<span data-ttu-id="11eef-123">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="11eef-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```




