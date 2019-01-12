---
title: windowsInformationProtectionApp-Ressourcentyp
description: App für Windows-Informationsschutz
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 270dd0b6328cd8290e656e46a0ff40551d2a5cbf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917797"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="91157-103">windowsInformationProtectionApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="91157-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="91157-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="91157-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91157-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="91157-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91157-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="91157-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91157-107">App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="91157-107">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="91157-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="91157-108">Properties</span></span>
|<span data-ttu-id="91157-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="91157-109">Property</span></span>|<span data-ttu-id="91157-110">Typ</span><span class="sxs-lookup"><span data-stu-id="91157-110">Type</span></span>|<span data-ttu-id="91157-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="91157-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91157-112">displayName</span><span class="sxs-lookup"><span data-stu-id="91157-112">displayName</span></span>|<span data-ttu-id="91157-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91157-113">String</span></span>|<span data-ttu-id="91157-114">Anzeigename der App</span><span class="sxs-lookup"><span data-stu-id="91157-114">App display name.</span></span>|
|<span data-ttu-id="91157-115">description</span><span class="sxs-lookup"><span data-stu-id="91157-115">description</span></span>|<span data-ttu-id="91157-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91157-116">String</span></span>|<span data-ttu-id="91157-117">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="91157-117">The app's description.</span></span>|
|<span data-ttu-id="91157-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="91157-118">publisherName</span></span>|<span data-ttu-id="91157-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91157-119">String</span></span>|<span data-ttu-id="91157-120">Name des Verlegers</span><span class="sxs-lookup"><span data-stu-id="91157-120">The publisher name</span></span>|
|<span data-ttu-id="91157-121">productName</span><span class="sxs-lookup"><span data-stu-id="91157-121">productName</span></span>|<span data-ttu-id="91157-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="91157-122">String</span></span>|<span data-ttu-id="91157-123">Produktname</span><span class="sxs-lookup"><span data-stu-id="91157-123">The product name.</span></span>|
|<span data-ttu-id="91157-124">denied</span><span class="sxs-lookup"><span data-stu-id="91157-124">denied</span></span>|<span data-ttu-id="91157-125">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="91157-125">Boolean</span></span>|<span data-ttu-id="91157-126">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="91157-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91157-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="91157-127">Relationships</span></span>
<span data-ttu-id="91157-128">Keine</span><span class="sxs-lookup"><span data-stu-id="91157-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91157-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="91157-129">JSON Representation</span></span>
<span data-ttu-id="91157-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="91157-130">Here is a JSON representation of the resource.</span></span>
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





