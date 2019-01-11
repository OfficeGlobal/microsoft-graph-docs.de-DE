---
title: windowsInformationProtectionApp-Ressourcentyp
description: App für Windows-Informationsschutz
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d44aa233e03a193ea0d061f55748cb0d7319a95b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809590"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="966ff-103">windowsInformationProtectionApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="966ff-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="966ff-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="966ff-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="966ff-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="966ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="966ff-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="966ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="966ff-107">App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="966ff-107">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="966ff-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="966ff-108">Properties</span></span>
|<span data-ttu-id="966ff-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="966ff-109">Property</span></span>|<span data-ttu-id="966ff-110">Typ</span><span class="sxs-lookup"><span data-stu-id="966ff-110">Type</span></span>|<span data-ttu-id="966ff-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="966ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="966ff-112">displayName</span><span class="sxs-lookup"><span data-stu-id="966ff-112">displayName</span></span>|<span data-ttu-id="966ff-113">String</span><span class="sxs-lookup"><span data-stu-id="966ff-113">String</span></span>|<span data-ttu-id="966ff-114">Anzeigename der App</span><span class="sxs-lookup"><span data-stu-id="966ff-114">App display name.</span></span>|
|<span data-ttu-id="966ff-115">description</span><span class="sxs-lookup"><span data-stu-id="966ff-115">description</span></span>|<span data-ttu-id="966ff-116">String</span><span class="sxs-lookup"><span data-stu-id="966ff-116">String</span></span>|<span data-ttu-id="966ff-117">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="966ff-117">The app's description.</span></span>|
|<span data-ttu-id="966ff-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="966ff-118">publisherName</span></span>|<span data-ttu-id="966ff-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="966ff-119">String</span></span>|<span data-ttu-id="966ff-120">Name des Verlegers</span><span class="sxs-lookup"><span data-stu-id="966ff-120">The publisher name</span></span>|
|<span data-ttu-id="966ff-121">productName</span><span class="sxs-lookup"><span data-stu-id="966ff-121">productName</span></span>|<span data-ttu-id="966ff-122">String</span><span class="sxs-lookup"><span data-stu-id="966ff-122">String</span></span>|<span data-ttu-id="966ff-123">Produktname</span><span class="sxs-lookup"><span data-stu-id="966ff-123">The product name.</span></span>|
|<span data-ttu-id="966ff-124">denied</span><span class="sxs-lookup"><span data-stu-id="966ff-124">denied</span></span>|<span data-ttu-id="966ff-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="966ff-125">Boolean</span></span>|<span data-ttu-id="966ff-126">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="966ff-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="966ff-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="966ff-127">Relationships</span></span>
<span data-ttu-id="966ff-128">Keine</span><span class="sxs-lookup"><span data-stu-id="966ff-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="966ff-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="966ff-129">JSON Representation</span></span>
<span data-ttu-id="966ff-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="966ff-130">Here is a JSON representation of the resource.</span></span>
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





