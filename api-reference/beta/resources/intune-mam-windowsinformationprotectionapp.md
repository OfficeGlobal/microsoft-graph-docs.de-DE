---
title: windowsInformationProtectionApp-Ressourcentyp
description: App für Windows-Informationsschutz
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 45d428ee18e92e76f5a13c568373219f904fd886
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403686"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="58b45-103">windowsInformationProtectionApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="58b45-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="58b45-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="58b45-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="58b45-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58b45-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58b45-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="58b45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58b45-107">App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="58b45-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="58b45-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="58b45-108">Properties</span></span>
|<span data-ttu-id="58b45-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58b45-109">Property</span></span>|<span data-ttu-id="58b45-110">Typ</span><span class="sxs-lookup"><span data-stu-id="58b45-110">Type</span></span>|<span data-ttu-id="58b45-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58b45-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58b45-112">displayName</span><span class="sxs-lookup"><span data-stu-id="58b45-112">displayName</span></span>|<span data-ttu-id="58b45-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58b45-113">String</span></span>|<span data-ttu-id="58b45-114">Anzeigename der App</span><span class="sxs-lookup"><span data-stu-id="58b45-114">App display name.</span></span>|
|<span data-ttu-id="58b45-115">description</span><span class="sxs-lookup"><span data-stu-id="58b45-115">description</span></span>|<span data-ttu-id="58b45-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58b45-116">String</span></span>|<span data-ttu-id="58b45-117">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="58b45-117">The app's description.</span></span>|
|<span data-ttu-id="58b45-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="58b45-118">publisherName</span></span>|<span data-ttu-id="58b45-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58b45-119">String</span></span>|<span data-ttu-id="58b45-120">Name des Verlegers</span><span class="sxs-lookup"><span data-stu-id="58b45-120">The publisher name</span></span>|
|<span data-ttu-id="58b45-121">productName</span><span class="sxs-lookup"><span data-stu-id="58b45-121">productName</span></span>|<span data-ttu-id="58b45-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58b45-122">String</span></span>|<span data-ttu-id="58b45-123">Produktname</span><span class="sxs-lookup"><span data-stu-id="58b45-123">The product name.</span></span>|
|<span data-ttu-id="58b45-124">denied</span><span class="sxs-lookup"><span data-stu-id="58b45-124">denied</span></span>|<span data-ttu-id="58b45-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="58b45-125">Boolean</span></span>|<span data-ttu-id="58b45-126">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="58b45-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58b45-127">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="58b45-127">Relationships</span></span>
<span data-ttu-id="58b45-128">Keine</span><span class="sxs-lookup"><span data-stu-id="58b45-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58b45-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="58b45-129">JSON Representation</span></span>
<span data-ttu-id="58b45-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="58b45-130">Here is a JSON representation of the resource.</span></span>
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




