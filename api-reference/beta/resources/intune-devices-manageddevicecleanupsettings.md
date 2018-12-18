---
title: Ressourcentyp managedDeviceCleanupSettings
description: Definieren Sie die Regel aus, wenn der Administrator die Geräte bereinigt werden möchte.
author: tfitzmac
ms.openlocfilehash: 84650c4d2d182fe0da30ced56786a2c0216a6358
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304088"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="fc539-103">Ressourcentyp managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="fc539-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="fc539-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fc539-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc539-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fc539-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc539-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fc539-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc539-107">Definieren Sie die Regel aus, wenn der Administrator die Geräte bereinigt werden möchte.</span><span class="sxs-lookup"><span data-stu-id="fc539-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="fc539-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fc539-108">Properties</span></span>
|<span data-ttu-id="fc539-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fc539-109">Property</span></span>|<span data-ttu-id="fc539-110">Typ</span><span class="sxs-lookup"><span data-stu-id="fc539-110">Type</span></span>|<span data-ttu-id="fc539-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc539-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc539-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="fc539-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="fc539-113">String</span><span class="sxs-lookup"><span data-stu-id="fc539-113">String</span></span>|<span data-ttu-id="fc539-114">Anzahl der Tage, wenn das Gerät nicht Intune kontaktiert hat.</span><span class="sxs-lookup"><span data-stu-id="fc539-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc539-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fc539-115">Relationships</span></span>
<span data-ttu-id="fc539-116">Keine</span><span class="sxs-lookup"><span data-stu-id="fc539-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fc539-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fc539-117">JSON Representation</span></span>
<span data-ttu-id="fc539-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fc539-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```





