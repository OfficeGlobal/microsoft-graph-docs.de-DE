---
title: windowsInformationProtectionApp-Ressourcentyp
description: App für Windows-Informationsschutz
ms.openlocfilehash: 0ea48e087d4a8450ee47b2239b7c67f3b050da85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016683"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="62f59-103">windowsInformationProtectionApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="62f59-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="62f59-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="62f59-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62f59-105">App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="62f59-105">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="62f59-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="62f59-106">Properties</span></span>
|<span data-ttu-id="62f59-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="62f59-107">Property</span></span>|<span data-ttu-id="62f59-108">Typ</span><span class="sxs-lookup"><span data-stu-id="62f59-108">Type</span></span>|<span data-ttu-id="62f59-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62f59-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62f59-110">displayName</span><span class="sxs-lookup"><span data-stu-id="62f59-110">displayName</span></span>|<span data-ttu-id="62f59-111">String</span><span class="sxs-lookup"><span data-stu-id="62f59-111">String</span></span>|<span data-ttu-id="62f59-112">Anzeigename der App</span><span class="sxs-lookup"><span data-stu-id="62f59-112">App display name.</span></span>|
|<span data-ttu-id="62f59-113">description</span><span class="sxs-lookup"><span data-stu-id="62f59-113">description</span></span>|<span data-ttu-id="62f59-114">String</span><span class="sxs-lookup"><span data-stu-id="62f59-114">String</span></span>|<span data-ttu-id="62f59-115">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="62f59-115">The app's description.</span></span>|
|<span data-ttu-id="62f59-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="62f59-116">publisherName</span></span>|<span data-ttu-id="62f59-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="62f59-117">String</span></span>|<span data-ttu-id="62f59-118">Name des Verlegers</span><span class="sxs-lookup"><span data-stu-id="62f59-118">The publisher name</span></span>|
|<span data-ttu-id="62f59-119">productName</span><span class="sxs-lookup"><span data-stu-id="62f59-119">productName</span></span>|<span data-ttu-id="62f59-120">String</span><span class="sxs-lookup"><span data-stu-id="62f59-120">String</span></span>|<span data-ttu-id="62f59-121">Produktname</span><span class="sxs-lookup"><span data-stu-id="62f59-121">The product name.</span></span>|
|<span data-ttu-id="62f59-122">denied</span><span class="sxs-lookup"><span data-stu-id="62f59-122">denied</span></span>|<span data-ttu-id="62f59-123">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="62f59-123">Boolean</span></span>|<span data-ttu-id="62f59-124">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="62f59-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62f59-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="62f59-125">Relationships</span></span>
<span data-ttu-id="62f59-126">Keine</span><span class="sxs-lookup"><span data-stu-id="62f59-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="62f59-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="62f59-127">JSON Representation</span></span>
<span data-ttu-id="62f59-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="62f59-128">Here is a JSON representation of the resource.</span></span>
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



