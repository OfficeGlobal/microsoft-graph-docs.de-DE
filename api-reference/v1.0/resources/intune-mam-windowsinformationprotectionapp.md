---
title: windowsInformationProtectionApp-Ressourcentyp
description: App für Windows-Informationsschutz
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00d329baea829fa8fb7664895382a377f53461ab
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257036"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="d7535-103">windowsInformationProtectionApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d7535-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="d7535-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d7535-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7535-105">App für Windows-Informationsschutz</span><span class="sxs-lookup"><span data-stu-id="d7535-105">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="d7535-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d7535-106">Properties</span></span>
|<span data-ttu-id="d7535-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d7535-107">Property</span></span>|<span data-ttu-id="d7535-108">Typ</span><span class="sxs-lookup"><span data-stu-id="d7535-108">Type</span></span>|<span data-ttu-id="d7535-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7535-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7535-110">displayName</span><span class="sxs-lookup"><span data-stu-id="d7535-110">displayName</span></span>|<span data-ttu-id="d7535-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d7535-111">String</span></span>|<span data-ttu-id="d7535-112">Anzeigename der App</span><span class="sxs-lookup"><span data-stu-id="d7535-112">App display name.</span></span>|
|<span data-ttu-id="d7535-113">description</span><span class="sxs-lookup"><span data-stu-id="d7535-113">description</span></span>|<span data-ttu-id="d7535-114">String</span><span class="sxs-lookup"><span data-stu-id="d7535-114">String</span></span>|<span data-ttu-id="d7535-115">Beschreibung der App</span><span class="sxs-lookup"><span data-stu-id="d7535-115">The app's description.</span></span>|
|<span data-ttu-id="d7535-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="d7535-116">publisherName</span></span>|<span data-ttu-id="d7535-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d7535-117">String</span></span>|<span data-ttu-id="d7535-118">Name des Verlegers</span><span class="sxs-lookup"><span data-stu-id="d7535-118">The publisher name</span></span>|
|<span data-ttu-id="d7535-119">productName</span><span class="sxs-lookup"><span data-stu-id="d7535-119">productName</span></span>|<span data-ttu-id="d7535-120">String</span><span class="sxs-lookup"><span data-stu-id="d7535-120">String</span></span>|<span data-ttu-id="d7535-121">Produktname</span><span class="sxs-lookup"><span data-stu-id="d7535-121">The product name.</span></span>|
|<span data-ttu-id="d7535-122">denied</span><span class="sxs-lookup"><span data-stu-id="d7535-122">denied</span></span>|<span data-ttu-id="d7535-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7535-123">Boolean</span></span>|<span data-ttu-id="d7535-124">Bei „true“ wird der App der Schutz oder eine Ausnahme verweigert.</span><span class="sxs-lookup"><span data-stu-id="d7535-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7535-125">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d7535-125">Relationships</span></span>
<span data-ttu-id="d7535-126">Keine</span><span class="sxs-lookup"><span data-stu-id="d7535-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7535-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d7535-127">JSON Representation</span></span>
<span data-ttu-id="d7535-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d7535-128">Here is a JSON representation of the resource.</span></span>
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



