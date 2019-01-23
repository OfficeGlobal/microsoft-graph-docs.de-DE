---
title: Ressourcentyp edgeHomeButtonOpensCustomURL
description: Zeigen Sie die Schaltfläche Startseite. durch Klicken auf die Schaltfläche Startseite lädt eine bestimmte URL.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 06f73375772f53b546e7e9b758a7513366949326
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431585"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="d4c5c-103">Ressourcentyp edgeHomeButtonOpensCustomURL</span><span class="sxs-lookup"><span data-stu-id="d4c5c-103">edgeHomeButtonOpensCustomURL resource type</span></span>

> <span data-ttu-id="d4c5c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4c5c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4c5c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4c5c-107">Zeigen Sie die Schaltfläche Startseite. durch Klicken auf die Schaltfläche Startseite lädt eine bestimmte URL.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="d4c5c-108">Erbt vom [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d4c5c-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d4c5c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d4c5c-109">Properties</span></span>
|<span data-ttu-id="d4c5c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4c5c-110">Property</span></span>|<span data-ttu-id="d4c5c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="d4c5c-111">Type</span></span>|<span data-ttu-id="d4c5c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4c5c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4c5c-113">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="d4c5c-113">homeButtonCustomURL</span></span>|<span data-ttu-id="d4c5c-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4c5c-114">String</span></span>|<span data-ttu-id="d4c5c-115">Die spezifischen URL zu laden.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4c5c-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d4c5c-116">Relationships</span></span>
<span data-ttu-id="d4c5c-117">Keine</span><span class="sxs-lookup"><span data-stu-id="d4c5c-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4c5c-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d4c5c-118">JSON Representation</span></span>
<span data-ttu-id="d4c5c-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d4c5c-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```




