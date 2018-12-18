---
title: Ressourcentyp windowsManagementAppHealthSummary
description: Enthält Eigenschaften für die Integrität Zusammenfassung der Windows Management-app.
author: tfitzmac
ms.openlocfilehash: 5717f96cbac534f2726ccf7bcfcbdb54d4c17b28
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326229"
---
# <a name="windowsmanagementapphealthsummary-resource-type"></a><span data-ttu-id="92ab8-103">Ressourcentyp windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="92ab8-103">windowsManagementAppHealthSummary resource type</span></span>

> <span data-ttu-id="92ab8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="92ab8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92ab8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92ab8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92ab8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="92ab8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92ab8-107">Enthält Eigenschaften für die Integrität Zusammenfassung der Windows Management-app.</span><span class="sxs-lookup"><span data-stu-id="92ab8-107">Contains properties for the health summary of the Windows management app.</span></span>
## <a name="methods"></a><span data-ttu-id="92ab8-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="92ab8-108">Methods</span></span>
|<span data-ttu-id="92ab8-109">Methode</span><span class="sxs-lookup"><span data-stu-id="92ab8-109">Method</span></span>|<span data-ttu-id="92ab8-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="92ab8-110">Return Type</span></span>|<span data-ttu-id="92ab8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92ab8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="92ab8-112">Abrufen von windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="92ab8-112">Get windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-get.md)|[<span data-ttu-id="92ab8-113">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="92ab8-113">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="92ab8-114">Lesen Sie Eigenschaften und Beziehungen des [WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="92ab8-114">Read properties and relationships of the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|
|[<span data-ttu-id="92ab8-115">WindowsManagementAppHealthSummary aktualisieren</span><span class="sxs-lookup"><span data-stu-id="92ab8-115">Update windowsManagementAppHealthSummary</span></span>](../api/intune-devices-windowsmanagementapphealthsummary-update.md)|[<span data-ttu-id="92ab8-116">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="92ab8-116">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="92ab8-117">Aktualisieren Sie die Eigenschaften eines [WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="92ab8-117">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="92ab8-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="92ab8-118">Properties</span></span>
|<span data-ttu-id="92ab8-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="92ab8-119">Property</span></span>|<span data-ttu-id="92ab8-120">Typ</span><span class="sxs-lookup"><span data-stu-id="92ab8-120">Type</span></span>|<span data-ttu-id="92ab8-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="92ab8-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92ab8-122">id</span><span class="sxs-lookup"><span data-stu-id="92ab8-122">id</span></span>|<span data-ttu-id="92ab8-123">String</span><span class="sxs-lookup"><span data-stu-id="92ab8-123">String</span></span>|<span data-ttu-id="92ab8-124">Schlüssel der Windows Management app Health Zusammenfassung Entität.</span><span class="sxs-lookup"><span data-stu-id="92ab8-124">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="92ab8-125">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="92ab8-125">healthyDeviceCount</span></span>|<span data-ttu-id="92ab8-126">Int32</span><span class="sxs-lookup"><span data-stu-id="92ab8-126">Int32</span></span>|<span data-ttu-id="92ab8-127">Anzahl der fehlerfrei Geräte.</span><span class="sxs-lookup"><span data-stu-id="92ab8-127">Healthy device count.</span></span>|
|<span data-ttu-id="92ab8-128">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="92ab8-128">unhealthyDeviceCount</span></span>|<span data-ttu-id="92ab8-129">Int32</span><span class="sxs-lookup"><span data-stu-id="92ab8-129">Int32</span></span>|<span data-ttu-id="92ab8-130">Anzahl der fehlerhaften Geräte.</span><span class="sxs-lookup"><span data-stu-id="92ab8-130">Unhealthy device count.</span></span>|
|<span data-ttu-id="92ab8-131">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="92ab8-131">unknownDeviceCount</span></span>|<span data-ttu-id="92ab8-132">Int32</span><span class="sxs-lookup"><span data-stu-id="92ab8-132">Int32</span></span>|<span data-ttu-id="92ab8-133">Anzahl der unbekannten Geräte.</span><span class="sxs-lookup"><span data-stu-id="92ab8-133">Unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92ab8-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="92ab8-134">Relationships</span></span>
<span data-ttu-id="92ab8-135">Keine</span><span class="sxs-lookup"><span data-stu-id="92ab8-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="92ab8-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="92ab8-136">JSON Representation</span></span>
<span data-ttu-id="92ab8-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="92ab8-137">Here is a JSON representation of the resource.</span></span>
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





