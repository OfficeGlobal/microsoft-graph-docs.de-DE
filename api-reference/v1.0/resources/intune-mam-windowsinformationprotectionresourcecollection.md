---
title: windowsInformationProtectionResourceCollection-Ressourcentyp
description: Windows Information Protection – Ressourcensammlung
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a913f90c2fed24a524e07b8dca1b629ebd9795f6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981217"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="12ee7-103">windowsInformationProtectionResourceCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="12ee7-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="12ee7-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="12ee7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12ee7-105">Windows Information Protection – Ressourcensammlung</span><span class="sxs-lookup"><span data-stu-id="12ee7-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="12ee7-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="12ee7-106">Properties</span></span>
|<span data-ttu-id="12ee7-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="12ee7-107">Property</span></span>|<span data-ttu-id="12ee7-108">Typ</span><span class="sxs-lookup"><span data-stu-id="12ee7-108">Type</span></span>|<span data-ttu-id="12ee7-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="12ee7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12ee7-110">displayName</span><span class="sxs-lookup"><span data-stu-id="12ee7-110">displayName</span></span>|<span data-ttu-id="12ee7-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="12ee7-111">String</span></span>|<span data-ttu-id="12ee7-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="12ee7-112">Display name</span></span>|
|<span data-ttu-id="12ee7-113">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="12ee7-113">resources</span></span>|<span data-ttu-id="12ee7-114">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="12ee7-114">String collection</span></span>|<span data-ttu-id="12ee7-115">Sammlung von Ressourcen</span><span class="sxs-lookup"><span data-stu-id="12ee7-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="12ee7-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="12ee7-116">Relationships</span></span>
<span data-ttu-id="12ee7-117">Keine</span><span class="sxs-lookup"><span data-stu-id="12ee7-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="12ee7-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="12ee7-118">JSON Representation</span></span>
<span data-ttu-id="12ee7-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="12ee7-119">Here is a JSON representation of the resource.</span></span>
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



