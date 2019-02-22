---
title: loggedOnUser-Ressourcentyp
description: AnGemeldeter Benutzer
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a5dfaa8bbaa879fc48c5f6ea31d1b7b14e998820
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148930"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="987bb-103">loggedOnUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="987bb-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="987bb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="987bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="987bb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="987bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="987bb-106">AnGemeldeter Benutzer</span><span class="sxs-lookup"><span data-stu-id="987bb-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="987bb-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="987bb-107">Properties</span></span>
|<span data-ttu-id="987bb-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="987bb-108">Property</span></span>|<span data-ttu-id="987bb-109">Typ</span><span class="sxs-lookup"><span data-stu-id="987bb-109">Type</span></span>|<span data-ttu-id="987bb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="987bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="987bb-111">userId</span><span class="sxs-lookup"><span data-stu-id="987bb-111">userId</span></span>|<span data-ttu-id="987bb-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="987bb-112">String</span></span>|<span data-ttu-id="987bb-113">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="987bb-113">User id</span></span>|
|<span data-ttu-id="987bb-114">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="987bb-114">lastLogOnDateTime</span></span>|<span data-ttu-id="987bb-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="987bb-115">DateTimeOffset</span></span>|<span data-ttu-id="987bb-116">Datum, an dem sich der Benutzer anmeldet</span><span class="sxs-lookup"><span data-stu-id="987bb-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="987bb-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="987bb-117">Relationships</span></span>
<span data-ttu-id="987bb-118">Keine</span><span class="sxs-lookup"><span data-stu-id="987bb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="987bb-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="987bb-119">JSON Representation</span></span>
<span data-ttu-id="987bb-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="987bb-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```




