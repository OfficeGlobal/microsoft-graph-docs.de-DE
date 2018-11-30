---
title: Ressourcentyp managedDeviceReportedApp
description: Anwendungsdaten für die berichterstellung
ms.openlocfilehash: 820269422891e01352a7f605d62147a84facea67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058975"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="84fda-103">Ressourcentyp managedDeviceReportedApp</span><span class="sxs-lookup"><span data-stu-id="84fda-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="84fda-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="84fda-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84fda-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84fda-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84fda-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="84fda-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84fda-107">Anwendungsdaten für die berichterstellung</span><span class="sxs-lookup"><span data-stu-id="84fda-107">Application data for reporting</span></span>
## <a name="properties"></a><span data-ttu-id="84fda-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="84fda-108">Properties</span></span>
|<span data-ttu-id="84fda-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="84fda-109">Property</span></span>|<span data-ttu-id="84fda-110">Typ</span><span class="sxs-lookup"><span data-stu-id="84fda-110">Type</span></span>|<span data-ttu-id="84fda-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="84fda-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84fda-112">appId</span><span class="sxs-lookup"><span data-stu-id="84fda-112">appId</span></span>|<span data-ttu-id="84fda-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="84fda-113">String</span></span>|<span data-ttu-id="84fda-114">Anwendungs- oder Paket-ID der Anwendung</span><span class="sxs-lookup"><span data-stu-id="84fda-114">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="84fda-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="84fda-115">Relationships</span></span>
<span data-ttu-id="84fda-116">Keine</span><span class="sxs-lookup"><span data-stu-id="84fda-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="84fda-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="84fda-117">JSON Representation</span></span>
<span data-ttu-id="84fda-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="84fda-118">Here is a JSON representation of the resource.</span></span>
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





