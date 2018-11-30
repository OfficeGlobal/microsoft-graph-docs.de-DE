---
title: windowsInformationProtectionResourceCollection-Ressourcentyp
description: Windows Information Protection – Ressourcensammlung
ms.openlocfilehash: fd350f85acb962267f92352e6298dc50c44949ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017680"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="d1885-103">windowsInformationProtectionResourceCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d1885-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="d1885-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d1885-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1885-105">Windows Information Protection – Ressourcensammlung</span><span class="sxs-lookup"><span data-stu-id="d1885-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="d1885-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d1885-106">Properties</span></span>
|<span data-ttu-id="d1885-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d1885-107">Property</span></span>|<span data-ttu-id="d1885-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d1885-108">Type</span></span>|<span data-ttu-id="d1885-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1885-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1885-110">displayName</span><span class="sxs-lookup"><span data-stu-id="d1885-110">displayName</span></span>|<span data-ttu-id="d1885-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1885-111">String</span></span>|<span data-ttu-id="d1885-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="d1885-112">Display name</span></span>|
|<span data-ttu-id="d1885-113">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="d1885-113">resources</span></span>|<span data-ttu-id="d1885-114">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="d1885-114">String collection</span></span>|<span data-ttu-id="d1885-115">Sammlung von Ressourcen</span><span class="sxs-lookup"><span data-stu-id="d1885-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1885-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d1885-116">Relationships</span></span>
<span data-ttu-id="d1885-117">Keine</span><span class="sxs-lookup"><span data-stu-id="d1885-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d1885-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d1885-118">JSON Representation</span></span>
<span data-ttu-id="d1885-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d1885-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```



