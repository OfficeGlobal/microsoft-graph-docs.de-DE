---
title: Ressourcentyp windows10AssociatedApps
description: Definition der Windows-10-Anwendung verknüpft ist.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 097edb32ca01d673bb4d42802e8588edd20cf2d1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869622"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="271c2-103">Ressourcentyp windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="271c2-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="271c2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="271c2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="271c2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="271c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="271c2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="271c2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="271c2-107">Definition der Windows-10-Anwendung verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="271c2-107">Windows 10 Associated Application definition.</span></span>
## <a name="properties"></a><span data-ttu-id="271c2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="271c2-108">Properties</span></span>
|<span data-ttu-id="271c2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="271c2-109">Property</span></span>|<span data-ttu-id="271c2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="271c2-110">Type</span></span>|<span data-ttu-id="271c2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="271c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="271c2-112">der appType</span><span class="sxs-lookup"><span data-stu-id="271c2-112">appType</span></span>|[<span data-ttu-id="271c2-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="271c2-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="271c2-114">Anwendungstyp.</span><span class="sxs-lookup"><span data-stu-id="271c2-114">Application type.</span></span> <span data-ttu-id="271c2-115">Mögliche Werte sind: `desktop` und `universal`.</span><span class="sxs-lookup"><span data-stu-id="271c2-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="271c2-116">Bezeichner</span><span class="sxs-lookup"><span data-stu-id="271c2-116">identifier</span></span>|<span data-ttu-id="271c2-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="271c2-117">String</span></span>|<span data-ttu-id="271c2-118">Bezeichner.</span><span class="sxs-lookup"><span data-stu-id="271c2-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="271c2-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="271c2-119">Relationships</span></span>
<span data-ttu-id="271c2-120">Keine</span><span class="sxs-lookup"><span data-stu-id="271c2-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="271c2-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="271c2-121">JSON Representation</span></span>
<span data-ttu-id="271c2-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="271c2-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```





