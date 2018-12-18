---
title: windowsInformationProtectionResourceCollection-Ressourcentyp
description: Windows Information Protection – Ressourcensammlung
author: tfitzmac
ms.openlocfilehash: 8e037ff53e11566aee7d79d2c3bbe5b1075b83a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327832"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="42560-103">windowsInformationProtectionResourceCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="42560-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="42560-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="42560-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42560-105">Windows Information Protection – Ressourcensammlung</span><span class="sxs-lookup"><span data-stu-id="42560-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="42560-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="42560-106">Properties</span></span>
|<span data-ttu-id="42560-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="42560-107">Property</span></span>|<span data-ttu-id="42560-108">Typ</span><span class="sxs-lookup"><span data-stu-id="42560-108">Type</span></span>|<span data-ttu-id="42560-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42560-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42560-110">displayName</span><span class="sxs-lookup"><span data-stu-id="42560-110">displayName</span></span>|<span data-ttu-id="42560-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="42560-111">String</span></span>|<span data-ttu-id="42560-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="42560-112">Display name</span></span>|
|<span data-ttu-id="42560-113">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="42560-113">resources</span></span>|<span data-ttu-id="42560-114">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="42560-114">String collection</span></span>|<span data-ttu-id="42560-115">Sammlung von Ressourcen</span><span class="sxs-lookup"><span data-stu-id="42560-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="42560-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="42560-116">Relationships</span></span>
<span data-ttu-id="42560-117">Keine</span><span class="sxs-lookup"><span data-stu-id="42560-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="42560-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="42560-118">JSON Representation</span></span>
<span data-ttu-id="42560-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="42560-119">Here is a JSON representation of the resource.</span></span>
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



