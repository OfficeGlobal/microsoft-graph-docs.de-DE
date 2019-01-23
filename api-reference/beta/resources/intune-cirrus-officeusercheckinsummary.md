---
title: Ressourcentyp officeUserCheckinSummary
description: Entität, die Mandanten Einchecken Stats beschreibt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d44c978ff1442c98038bf627397de5ca3a0ca3bf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411008"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="b8e06-103">Ressourcentyp officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="b8e06-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="b8e06-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b8e06-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b8e06-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b8e06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8e06-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b8e06-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8e06-107">Entität, die Mandanten Einchecken Stats beschreibt.</span><span class="sxs-lookup"><span data-stu-id="b8e06-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="b8e06-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b8e06-108">Properties</span></span>
|<span data-ttu-id="b8e06-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8e06-109">Property</span></span>|<span data-ttu-id="b8e06-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b8e06-110">Type</span></span>|<span data-ttu-id="b8e06-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8e06-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8e06-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="b8e06-112">succeededUserCount</span></span>|<span data-ttu-id="b8e06-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e06-113">Int32</span></span>|<span data-ttu-id="b8e06-114">Gesamtzahl erfolgreicher Benutzer überprüfen ins für die letzten drei Monate angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b8e06-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="b8e06-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="b8e06-115">failedUserCount</span></span>|<span data-ttu-id="b8e06-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b8e06-116">Int32</span></span>|<span data-ttu-id="b8e06-117">Benutzer gesamt fehlgeschlagenen überprüfen ins für die letzten drei Monate angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b8e06-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8e06-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b8e06-118">Relationships</span></span>
<span data-ttu-id="b8e06-119">Keine</span><span class="sxs-lookup"><span data-stu-id="b8e06-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8e06-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b8e06-120">JSON Representation</span></span>
<span data-ttu-id="b8e06-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b8e06-121">Here is a JSON representation of the resource.</span></span>
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



