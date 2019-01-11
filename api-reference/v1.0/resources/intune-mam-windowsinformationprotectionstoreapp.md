---
title: windowsInformationProtectionStoreApp-Ressourcentyp
description: Store-App für Windows-Informationsschutz
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4e78aa854b15763cade9a4d6020f1737bbca1642
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814476"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="eb89f-103">windowsInformationProtectionStoreApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="eb89f-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="eb89f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eb89f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb89f-105">Store-App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="eb89f-105">Store App for Windows information protection</span></span>

<span data-ttu-id="eb89f-106">Erbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb89f-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb89f-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="eb89f-107">Properties</span></span>
|<span data-ttu-id="eb89f-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eb89f-108">Property</span></span>|<span data-ttu-id="eb89f-109">Typ</span><span class="sxs-lookup"><span data-stu-id="eb89f-109">Type</span></span>|<span data-ttu-id="eb89f-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb89f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb89f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="eb89f-111">displayName</span></span>|<span data-ttu-id="eb89f-112">String</span><span class="sxs-lookup"><span data-stu-id="eb89f-112">String</span></span>|<span data-ttu-id="eb89f-113">Anzeigename der App.</span><span class="sxs-lookup"><span data-stu-id="eb89f-113">App display name.</span></span> <span data-ttu-id="eb89f-114">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb89f-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb89f-115">description</span><span class="sxs-lookup"><span data-stu-id="eb89f-115">description</span></span>|<span data-ttu-id="eb89f-116">String</span><span class="sxs-lookup"><span data-stu-id="eb89f-116">String</span></span>|<span data-ttu-id="eb89f-117">Die Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="eb89f-117">The app's description.</span></span> <span data-ttu-id="eb89f-118">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb89f-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb89f-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="eb89f-119">publisherName</span></span>|<span data-ttu-id="eb89f-120">String</span><span class="sxs-lookup"><span data-stu-id="eb89f-120">String</span></span>|<span data-ttu-id="eb89f-121">Der Name des Herausgebers, geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb89f-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb89f-122">productName</span><span class="sxs-lookup"><span data-stu-id="eb89f-122">productName</span></span>|<span data-ttu-id="eb89f-123">String</span><span class="sxs-lookup"><span data-stu-id="eb89f-123">String</span></span>|<span data-ttu-id="eb89f-124">Der Produktname.</span><span class="sxs-lookup"><span data-stu-id="eb89f-124">The product name.</span></span> <span data-ttu-id="eb89f-125">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb89f-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb89f-126">denied</span><span class="sxs-lookup"><span data-stu-id="eb89f-126">denied</span></span>|<span data-ttu-id="eb89f-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="eb89f-127">Boolean</span></span>|<span data-ttu-id="eb89f-128">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="eb89f-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="eb89f-129">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb89f-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb89f-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="eb89f-130">Relationships</span></span>
<span data-ttu-id="eb89f-131">Keine</span><span class="sxs-lookup"><span data-stu-id="eb89f-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eb89f-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="eb89f-132">JSON Representation</span></span>
<span data-ttu-id="eb89f-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="eb89f-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



