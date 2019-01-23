---
title: Ressourcentyp managedDeviceReportedApp
description: Anwendungsdaten für die berichterstellung
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 104503083f5f599bc366de2ca8082fd9fdf3102e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422607"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="0f9bb-103">Ressourcentyp managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="0f9bb-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="0f9bb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0f9bb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0f9bb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f9bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f9bb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0f9bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f9bb-107">Anwendungsdaten für die berichterstellung</span><span class="sxs-lookup"><span data-stu-id="0f9bb-107">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="0f9bb-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0f9bb-108">Properties</span></span>
|<span data-ttu-id="0f9bb-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f9bb-109">Property</span></span>|<span data-ttu-id="0f9bb-110">Typ</span><span class="sxs-lookup"><span data-stu-id="0f9bb-110">Type</span></span>|<span data-ttu-id="0f9bb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f9bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f9bb-112">appId</span><span class="sxs-lookup"><span data-stu-id="0f9bb-112">appId</span></span>|<span data-ttu-id="0f9bb-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0f9bb-113">String</span></span>|<span data-ttu-id="0f9bb-114">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f9bb-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f9bb-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0f9bb-115">Relationships</span></span>
<span data-ttu-id="0f9bb-116">Keine</span><span class="sxs-lookup"><span data-stu-id="0f9bb-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f9bb-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0f9bb-117">JSON Representation</span></span>
<span data-ttu-id="0f9bb-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0f9bb-118">Here is a JSON representation of the resource.</span></span>
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




