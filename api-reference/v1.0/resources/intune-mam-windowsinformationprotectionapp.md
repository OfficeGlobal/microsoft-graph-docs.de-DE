---
title: windowsInformationProtectionApp-Ressourcentyp
description: App für Windows-Informationsschutz
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8d025b20e5341c17f756e86bb6bb84faf92a61a3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971879"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="e6239-103">windowsInformationProtectionApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e6239-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="e6239-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e6239-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6239-105">App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="e6239-105">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="e6239-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e6239-106">Properties</span></span>
|<span data-ttu-id="e6239-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e6239-107">Property</span></span>|<span data-ttu-id="e6239-108">Typ</span><span class="sxs-lookup"><span data-stu-id="e6239-108">Type</span></span>|<span data-ttu-id="e6239-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e6239-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6239-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e6239-110">displayName</span></span>|<span data-ttu-id="e6239-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6239-111">String</span></span>|<span data-ttu-id="e6239-112">Anzeigename der App</span><span class="sxs-lookup"><span data-stu-id="e6239-112">App display name.</span></span>|
|<span data-ttu-id="e6239-113">description</span><span class="sxs-lookup"><span data-stu-id="e6239-113">description</span></span>|<span data-ttu-id="e6239-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6239-114">String</span></span>|<span data-ttu-id="e6239-115">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="e6239-115">The app's description.</span></span>|
|<span data-ttu-id="e6239-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="e6239-116">publisherName</span></span>|<span data-ttu-id="e6239-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6239-117">String</span></span>|<span data-ttu-id="e6239-118">Name des Verlegers</span><span class="sxs-lookup"><span data-stu-id="e6239-118">The publisher name</span></span>|
|<span data-ttu-id="e6239-119">productName</span><span class="sxs-lookup"><span data-stu-id="e6239-119">productName</span></span>|<span data-ttu-id="e6239-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e6239-120">String</span></span>|<span data-ttu-id="e6239-121">Produktname</span><span class="sxs-lookup"><span data-stu-id="e6239-121">The product name.</span></span>|
|<span data-ttu-id="e6239-122">denied</span><span class="sxs-lookup"><span data-stu-id="e6239-122">denied</span></span>|<span data-ttu-id="e6239-123">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="e6239-123">Boolean</span></span>|<span data-ttu-id="e6239-124">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="e6239-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6239-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e6239-125">Relationships</span></span>
<span data-ttu-id="e6239-126">Keine</span><span class="sxs-lookup"><span data-stu-id="e6239-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e6239-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e6239-127">JSON Representation</span></span>
<span data-ttu-id="e6239-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e6239-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



