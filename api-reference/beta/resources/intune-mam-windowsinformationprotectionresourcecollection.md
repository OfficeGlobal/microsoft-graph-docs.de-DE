---
title: windowsInformationProtectionResourceCollection-Ressourcentyp
description: Windows Information Protection – Ressourcensammlung
author: tfitzmac
ms.openlocfilehash: 96b3b36f40d1eeb88731f6f44ebec812a18fe713
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306888"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="eb9fb-103">windowsInformationProtectionResourceCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="eb9fb-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="eb9fb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eb9fb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb9fb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eb9fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb9fb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eb9fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb9fb-107">Windows Information Protection – Ressourcensammlung</span><span class="sxs-lookup"><span data-stu-id="eb9fb-107">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="eb9fb-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eb9fb-108">Properties</span></span>
|<span data-ttu-id="eb9fb-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eb9fb-109">Property</span></span>|<span data-ttu-id="eb9fb-110">Typ</span><span class="sxs-lookup"><span data-stu-id="eb9fb-110">Type</span></span>|<span data-ttu-id="eb9fb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb9fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb9fb-112">displayName</span><span class="sxs-lookup"><span data-stu-id="eb9fb-112">displayName</span></span>|<span data-ttu-id="eb9fb-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb9fb-113">String</span></span>|<span data-ttu-id="eb9fb-114">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="eb9fb-114">Display name</span></span>|
|<span data-ttu-id="eb9fb-115">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="eb9fb-115">resources</span></span>|<span data-ttu-id="eb9fb-116">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="eb9fb-116">String collection</span></span>|<span data-ttu-id="eb9fb-117">Sammlung von Ressourcen</span><span class="sxs-lookup"><span data-stu-id="eb9fb-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb9fb-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="eb9fb-118">Relationships</span></span>
<span data-ttu-id="eb9fb-119">Keine</span><span class="sxs-lookup"><span data-stu-id="eb9fb-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eb9fb-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eb9fb-120">JSON Representation</span></span>
<span data-ttu-id="eb9fb-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eb9fb-121">Here is a JSON representation of the resource.</span></span>
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





