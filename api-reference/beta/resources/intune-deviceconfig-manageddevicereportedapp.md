---
title: Ressourcentyp managedDeviceReportedApp
description: Anwendungsdaten für die berichterstellung
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 676b89e98f5d54367916a3f3219ab5fc02ddbd80
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877217"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="17b94-103">Ressourcentyp managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="17b94-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="17b94-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="17b94-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17b94-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="17b94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17b94-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="17b94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17b94-107">Anwendungsdaten für die berichterstellung</span><span class="sxs-lookup"><span data-stu-id="17b94-107">Application data for reporting</span></span>
## <a name="properties"></a><span data-ttu-id="17b94-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="17b94-108">Properties</span></span>
|<span data-ttu-id="17b94-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="17b94-109">Property</span></span>|<span data-ttu-id="17b94-110">Typ</span><span class="sxs-lookup"><span data-stu-id="17b94-110">Type</span></span>|<span data-ttu-id="17b94-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="17b94-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17b94-112">appId</span><span class="sxs-lookup"><span data-stu-id="17b94-112">appId</span></span>|<span data-ttu-id="17b94-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="17b94-113">String</span></span>|<span data-ttu-id="17b94-114">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="17b94-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="17b94-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="17b94-115">Relationships</span></span>
<span data-ttu-id="17b94-116">Keine</span><span class="sxs-lookup"><span data-stu-id="17b94-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="17b94-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="17b94-117">JSON Representation</span></span>
<span data-ttu-id="17b94-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="17b94-118">Here is a JSON representation of the resource.</span></span>
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





