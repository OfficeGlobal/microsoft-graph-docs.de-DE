---
title: Intunebrand-Ressourcentyp
description: Informationen zur Administrator Einwilligung.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f46e379a47bd7b08be1427115c785452543dfbf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157939"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="16a0d-103">Intunebrand-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="16a0d-103">adminConsent resource type</span></span>

> <span data-ttu-id="16a0d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="16a0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16a0d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="16a0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16a0d-106">Informationen zur Administrator Einwilligung.</span><span class="sxs-lookup"><span data-stu-id="16a0d-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="16a0d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="16a0d-107">Properties</span></span>
|<span data-ttu-id="16a0d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="16a0d-108">Property</span></span>|<span data-ttu-id="16a0d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="16a0d-109">Type</span></span>|<span data-ttu-id="16a0d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="16a0d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16a0d-111">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="16a0d-111">shareAPNSData</span></span>|[<span data-ttu-id="16a0d-112">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="16a0d-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="16a0d-113">Der Administrator Einwilligungs Status der Freigabe von Benutzer-und Gerätedaten an Apple.</span><span class="sxs-lookup"><span data-stu-id="16a0d-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="16a0d-114">Mögliche Werte sind: `notConfigured`, `granted` und `notGranted`.</span><span class="sxs-lookup"><span data-stu-id="16a0d-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16a0d-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="16a0d-115">Relationships</span></span>
<span data-ttu-id="16a0d-116">Keine</span><span class="sxs-lookup"><span data-stu-id="16a0d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16a0d-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="16a0d-117">JSON Representation</span></span>
<span data-ttu-id="16a0d-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="16a0d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```




