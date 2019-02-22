---
title: extendedKeyUsage-Ressourcentyp
description: Definition der benutzerdefinierten erweiterten Schlüsselverwendung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1487d217693135e26df99d4d72491abac4123ba7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173290"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="642a3-103">extendedKeyUsage-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="642a3-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="642a3-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="642a3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="642a3-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="642a3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="642a3-106">Definition der benutzerdefinierten erweiterten Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="642a3-106">Custom Extended Key Usage definition</span></span>

## <a name="properties"></a><span data-ttu-id="642a3-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="642a3-107">Properties</span></span>
|<span data-ttu-id="642a3-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="642a3-108">Property</span></span>|<span data-ttu-id="642a3-109">Typ</span><span class="sxs-lookup"><span data-stu-id="642a3-109">Type</span></span>|<span data-ttu-id="642a3-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="642a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="642a3-111">name</span><span class="sxs-lookup"><span data-stu-id="642a3-111">name</span></span>|<span data-ttu-id="642a3-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="642a3-112">String</span></span>|<span data-ttu-id="642a3-113">Name der erweiterten Schlüsselverwendung</span><span class="sxs-lookup"><span data-stu-id="642a3-113">Extended Key Usage Name</span></span>|
|<span data-ttu-id="642a3-114">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="642a3-114">objectIdentifier</span></span>|<span data-ttu-id="642a3-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="642a3-115">String</span></span>|<span data-ttu-id="642a3-116">Bezeichner des erweiterten Schlüssel Verwendungs Objekts</span><span class="sxs-lookup"><span data-stu-id="642a3-116">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="642a3-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="642a3-117">Relationships</span></span>
<span data-ttu-id="642a3-118">Keine</span><span class="sxs-lookup"><span data-stu-id="642a3-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="642a3-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="642a3-119">JSON Representation</span></span>
<span data-ttu-id="642a3-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="642a3-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```




