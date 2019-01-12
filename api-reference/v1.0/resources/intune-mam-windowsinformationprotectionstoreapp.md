---
title: windowsInformationProtectionStoreApp-Ressourcentyp
description: Store-App für Windows-Informationsschutz
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90f89f46c81676a3f51b019df26eb042d3f5bd79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919421"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="d568d-103">windowsInformationProtectionStoreApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d568d-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="d568d-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d568d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d568d-105">Store-App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="d568d-105">Store App for Windows information protection</span></span>

<span data-ttu-id="d568d-106">Erbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d568d-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d568d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d568d-107">Properties</span></span>
|<span data-ttu-id="d568d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d568d-108">Property</span></span>|<span data-ttu-id="d568d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d568d-109">Type</span></span>|<span data-ttu-id="d568d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d568d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d568d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d568d-111">displayName</span></span>|<span data-ttu-id="d568d-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d568d-112">String</span></span>|<span data-ttu-id="d568d-113">Anzeigename der App.</span><span class="sxs-lookup"><span data-stu-id="d568d-113">App display name.</span></span> <span data-ttu-id="d568d-114">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d568d-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="d568d-115">description</span><span class="sxs-lookup"><span data-stu-id="d568d-115">description</span></span>|<span data-ttu-id="d568d-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d568d-116">String</span></span>|<span data-ttu-id="d568d-117">Die Beschreibung der App.</span><span class="sxs-lookup"><span data-stu-id="d568d-117">The app's description.</span></span> <span data-ttu-id="d568d-118">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d568d-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="d568d-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="d568d-119">publisherName</span></span>|<span data-ttu-id="d568d-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d568d-120">String</span></span>|<span data-ttu-id="d568d-121">Der Name des Herausgebers, geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d568d-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="d568d-122">productName</span><span class="sxs-lookup"><span data-stu-id="d568d-122">productName</span></span>|<span data-ttu-id="d568d-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d568d-123">String</span></span>|<span data-ttu-id="d568d-124">Der Produktname.</span><span class="sxs-lookup"><span data-stu-id="d568d-124">The product name.</span></span> <span data-ttu-id="d568d-125">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d568d-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="d568d-126">denied</span><span class="sxs-lookup"><span data-stu-id="d568d-126">denied</span></span>|<span data-ttu-id="d568d-127">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="d568d-127">Boolean</span></span>|<span data-ttu-id="d568d-128">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="d568d-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="d568d-129">Geerbt von [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="d568d-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d568d-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d568d-130">Relationships</span></span>
<span data-ttu-id="d568d-131">Keine</span><span class="sxs-lookup"><span data-stu-id="d568d-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d568d-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d568d-132">JSON Representation</span></span>
<span data-ttu-id="d568d-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d568d-133">Here is a JSON representation of the resource.</span></span>
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



