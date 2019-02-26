---
title: report-Ressourcentyp
description: Beschreibt die Berichtsressource der Microsoft Graph-API für InTune, die mehrere Workflows unterstützt.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: f523f6df0b8b90cb6649ac81f1e433d6df227aea
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165751"
---
# <a name="report-resource-type"></a><span data-ttu-id="4b346-103">report-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4b346-103">report resource type</span></span>

> <span data-ttu-id="4b346-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b346-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b346-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4b346-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b346-106">Gibt den für den Kontext geeigneten Inhalt zurück, einschließlich:</span><span class="sxs-lookup"><span data-stu-id="4b346-106">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="4b346-107">Verlaufsberichte für Geräte Konfigurationsprofile.</span><span class="sxs-lookup"><span data-stu-id="4b346-107">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="4b346-108">Berichte zur Registrierung.</span><span class="sxs-lookup"><span data-stu-id="4b346-108">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="4b346-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4b346-109">Properties</span></span>
|<span data-ttu-id="4b346-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b346-110">Property</span></span>|<span data-ttu-id="4b346-111">Typ</span><span class="sxs-lookup"><span data-stu-id="4b346-111">Type</span></span>|<span data-ttu-id="4b346-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b346-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b346-113">Inhalt</span><span class="sxs-lookup"><span data-stu-id="4b346-113">content</span></span>|<span data-ttu-id="4b346-114">Stream</span><span class="sxs-lookup"><span data-stu-id="4b346-114">Stream</span></span>|<span data-ttu-id="4b346-115">Berichtsinhalt; Details variieren je nach Berichtstyp.</span><span class="sxs-lookup"><span data-stu-id="4b346-115">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b346-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4b346-116">Relationships</span></span>
<span data-ttu-id="4b346-117">Keine</span><span class="sxs-lookup"><span data-stu-id="4b346-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b346-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4b346-118">JSON Representation</span></span>
<span data-ttu-id="4b346-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4b346-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



