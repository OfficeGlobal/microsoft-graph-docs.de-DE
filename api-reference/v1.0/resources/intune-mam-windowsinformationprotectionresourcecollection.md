---
title: windowsInformationProtectionResourceCollection-Ressourcentyp
description: Windows Information Protection – Ressourcensammlung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74d7549f57ecc59f70aa1af4350544ec21b156ec
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254821"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="3fd8b-103">windowsInformationProtectionResourceCollection-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3fd8b-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="3fd8b-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3fd8b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fd8b-105">Windows Information Protection – Ressourcensammlung</span><span class="sxs-lookup"><span data-stu-id="3fd8b-105">Windows Information Protection Resource Collection</span></span>

## <a name="properties"></a><span data-ttu-id="3fd8b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3fd8b-106">Properties</span></span>
|<span data-ttu-id="3fd8b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3fd8b-107">Property</span></span>|<span data-ttu-id="3fd8b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="3fd8b-108">Type</span></span>|<span data-ttu-id="3fd8b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3fd8b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fd8b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="3fd8b-110">displayName</span></span>|<span data-ttu-id="3fd8b-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3fd8b-111">String</span></span>|<span data-ttu-id="3fd8b-112">Anzeigename</span><span class="sxs-lookup"><span data-stu-id="3fd8b-112">Display name</span></span>|
|<span data-ttu-id="3fd8b-113">Ressourcen</span><span class="sxs-lookup"><span data-stu-id="3fd8b-113">resources</span></span>|<span data-ttu-id="3fd8b-114">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="3fd8b-114">String collection</span></span>|<span data-ttu-id="3fd8b-115">Sammlung von Ressourcen</span><span class="sxs-lookup"><span data-stu-id="3fd8b-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fd8b-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3fd8b-116">Relationships</span></span>
<span data-ttu-id="3fd8b-117">Keine</span><span class="sxs-lookup"><span data-stu-id="3fd8b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fd8b-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3fd8b-118">JSON Representation</span></span>
<span data-ttu-id="3fd8b-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3fd8b-119">Here is a JSON representation of the resource.</span></span>
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



