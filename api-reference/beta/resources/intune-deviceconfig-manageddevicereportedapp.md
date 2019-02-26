---
title: managedDeviceReportedApp-Ressourcentyp
description: Anwendungsdaten für die Berichterstellung
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3e1cd99974259835859cf8a2fc6a9f197c09d4d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166269"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="0f4d1-103">managedDeviceReportedApp-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0f4d1-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="0f4d1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f4d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f4d1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0f4d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f4d1-106">Anwendungsdaten für die Berichterstellung</span><span class="sxs-lookup"><span data-stu-id="0f4d1-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="0f4d1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f4d1-107">Properties</span></span>
|<span data-ttu-id="0f4d1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f4d1-108">Property</span></span>|<span data-ttu-id="0f4d1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="0f4d1-109">Type</span></span>|<span data-ttu-id="0f4d1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f4d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f4d1-111">appId</span><span class="sxs-lookup"><span data-stu-id="0f4d1-111">appId</span></span>|<span data-ttu-id="0f4d1-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f4d1-112">String</span></span>|<span data-ttu-id="0f4d1-113">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f4d1-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f4d1-114">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0f4d1-114">Relationships</span></span>
<span data-ttu-id="0f4d1-115">Keine</span><span class="sxs-lookup"><span data-stu-id="0f4d1-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f4d1-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f4d1-116">JSON Representation</span></span>
<span data-ttu-id="0f4d1-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f4d1-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceReportedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceReportedApp",
  "appId": "String"
}
```




