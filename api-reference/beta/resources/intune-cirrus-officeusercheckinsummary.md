---
title: officeUserCheckinSummary-Ressourcentyp
description: Entität, die den Eincheckstatus für Mandanten beschreibt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b74d7508c9ef3b1d7183c806783e567cb75859ff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143358"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="26216-103">officeUserCheckinSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="26216-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="26216-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="26216-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26216-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="26216-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26216-106">Entität, die den Eincheckstatus für Mandanten beschreibt.</span><span class="sxs-lookup"><span data-stu-id="26216-106">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="26216-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="26216-107">Properties</span></span>
|<span data-ttu-id="26216-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="26216-108">Property</span></span>|<span data-ttu-id="26216-109">Typ</span><span class="sxs-lookup"><span data-stu-id="26216-109">Type</span></span>|<span data-ttu-id="26216-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="26216-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26216-111">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="26216-111">succeededUserCount</span></span>|<span data-ttu-id="26216-112">Int32</span><span class="sxs-lookup"><span data-stu-id="26216-112">Int32</span></span>|<span data-ttu-id="26216-113">Erfolgreiche Einchecken von Benutzern für die letzten drei Monate.</span><span class="sxs-lookup"><span data-stu-id="26216-113">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="26216-114">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="26216-114">failedUserCount</span></span>|<span data-ttu-id="26216-115">Int32</span><span class="sxs-lookup"><span data-stu-id="26216-115">Int32</span></span>|<span data-ttu-id="26216-116">Insgesamt fehlgeschlagene Benutzer Einchecken für die letzten 3 Monate.</span><span class="sxs-lookup"><span data-stu-id="26216-116">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26216-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="26216-117">Relationships</span></span>
<span data-ttu-id="26216-118">Keine</span><span class="sxs-lookup"><span data-stu-id="26216-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26216-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="26216-119">JSON Representation</span></span>
<span data-ttu-id="26216-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="26216-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```



