---
title: windowsManagementAppHealthSummary-Ressourcentyp
description: Enthält Eigenschaften für die Integritäts Zusammenfassung der Windows-Verwaltungs-app.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f62f5967702143149176cecd2513478256ead6d3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172058"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="ae572-103">windowsManagementAppHealthSummary-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ae572-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="ae572-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae572-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae572-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ae572-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae572-106">Enthält Eigenschaften für die Integritäts Zusammenfassung der Windows-Verwaltungs-app.</span><span class="sxs-lookup"><span data-stu-id="ae572-106">Contains properties for the health summary of the Windows management app.</span></span>

## <a name="methods"></a><span data-ttu-id="ae572-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="ae572-107">Methods</span></span>
|<span data-ttu-id="ae572-108">Methode</span><span class="sxs-lookup"><span data-stu-id="ae572-108">Method</span></span>|<span data-ttu-id="ae572-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ae572-109">Return Type</span></span>|<span data-ttu-id="ae572-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae572-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ae572-111">WindowsManagementAppHealthSummary abrufen</span><span class="sxs-lookup"><span data-stu-id="ae572-111">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="ae572-112">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="ae572-112">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="ae572-113">Lesen von Eigenschaften und Beziehungen des [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae572-113">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="ae572-114">WindowsManagementAppHealthSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="ae572-114">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="ae572-115">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="ae572-115">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="ae572-116">Aktualisieren der Eigenschaften eines [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="ae572-116">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae572-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ae572-117">Properties</span></span>
|<span data-ttu-id="ae572-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ae572-118">Property</span></span>|<span data-ttu-id="ae572-119">Typ</span><span class="sxs-lookup"><span data-stu-id="ae572-119">Type</span></span>|<span data-ttu-id="ae572-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ae572-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae572-121">id</span><span class="sxs-lookup"><span data-stu-id="ae572-121">id</span></span>|<span data-ttu-id="ae572-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ae572-122">String</span></span>|<span data-ttu-id="ae572-123">Schlüssel der Status Zusammenfassungs Entität der Windows-Verwaltungs app.</span><span class="sxs-lookup"><span data-stu-id="ae572-123">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="ae572-124">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae572-124">healthyDeviceCount</span></span>|<span data-ttu-id="ae572-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ae572-125">Int32</span></span>|<span data-ttu-id="ae572-126">Anzahl der fehlerfreien Geräte.</span><span class="sxs-lookup"><span data-stu-id="ae572-126">Healthy device count.</span></span>|
|<span data-ttu-id="ae572-127">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae572-127">unhealthyDeviceCount</span></span>|<span data-ttu-id="ae572-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ae572-128">Int32</span></span>|<span data-ttu-id="ae572-129">Fehlerhafte Geräteanzahl.</span><span class="sxs-lookup"><span data-stu-id="ae572-129">Unhealthy device count.</span></span>|
|<span data-ttu-id="ae572-130">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae572-130">unknownDeviceCount</span></span>|<span data-ttu-id="ae572-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ae572-131">Int32</span></span>|<span data-ttu-id="ae572-132">Unbekannte Geräteanzahl.</span><span class="sxs-lookup"><span data-stu-id="ae572-132">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae572-133">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ae572-133">Relationships</span></span>
<span data-ttu-id="ae572-134">Keine</span><span class="sxs-lookup"><span data-stu-id="ae572-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae572-135">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ae572-135">JSON Representation</span></span>
<span data-ttu-id="ae572-136">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ae572-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "String (identifier)",
  "healthyDeviceCount": 1024,
  "unhealthyDeviceCount": 1024,
  "unknownDeviceCount": 1024
}
```




