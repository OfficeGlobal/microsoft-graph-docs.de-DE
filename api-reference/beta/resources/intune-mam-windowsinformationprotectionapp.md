---
title: windowsInformationProtectionApp-Ressourcentyp
description: App für Windows-Informationsschutz
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2b8739fd045d4b8e6293164fc7e9b14154a475c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139284"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="81d4b-103">windowsInformationProtectionApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="81d4b-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="81d4b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="81d4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81d4b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="81d4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81d4b-106">App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="81d4b-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="81d4b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="81d4b-107">Properties</span></span>
|<span data-ttu-id="81d4b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="81d4b-108">Property</span></span>|<span data-ttu-id="81d4b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="81d4b-109">Type</span></span>|<span data-ttu-id="81d4b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81d4b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81d4b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="81d4b-111">displayName</span></span>|<span data-ttu-id="81d4b-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81d4b-112">String</span></span>|<span data-ttu-id="81d4b-113">Anzeigename der App</span><span class="sxs-lookup"><span data-stu-id="81d4b-113">App display name.</span></span>|
|<span data-ttu-id="81d4b-114">description</span><span class="sxs-lookup"><span data-stu-id="81d4b-114">description</span></span>|<span data-ttu-id="81d4b-115">String</span><span class="sxs-lookup"><span data-stu-id="81d4b-115">String</span></span>|<span data-ttu-id="81d4b-116">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="81d4b-116">The app's description.</span></span>|
|<span data-ttu-id="81d4b-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="81d4b-117">publisherName</span></span>|<span data-ttu-id="81d4b-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81d4b-118">String</span></span>|<span data-ttu-id="81d4b-119">Name des Verlegers</span><span class="sxs-lookup"><span data-stu-id="81d4b-119">The publisher name</span></span>|
|<span data-ttu-id="81d4b-120">productName</span><span class="sxs-lookup"><span data-stu-id="81d4b-120">productName</span></span>|<span data-ttu-id="81d4b-121">String</span><span class="sxs-lookup"><span data-stu-id="81d4b-121">String</span></span>|<span data-ttu-id="81d4b-122">Produktname</span><span class="sxs-lookup"><span data-stu-id="81d4b-122">The product name.</span></span>|
|<span data-ttu-id="81d4b-123">denied</span><span class="sxs-lookup"><span data-stu-id="81d4b-123">denied</span></span>|<span data-ttu-id="81d4b-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="81d4b-124">Boolean</span></span>|<span data-ttu-id="81d4b-125">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="81d4b-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81d4b-126">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="81d4b-126">Relationships</span></span>
<span data-ttu-id="81d4b-127">Keine</span><span class="sxs-lookup"><span data-stu-id="81d4b-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81d4b-128">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="81d4b-128">JSON Representation</span></span>
<span data-ttu-id="81d4b-129">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="81d4b-129">Here is a JSON representation of the resource.</span></span>
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




