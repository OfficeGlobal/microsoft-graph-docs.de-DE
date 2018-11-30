---
title: Ressourcentyp managedDeviceCleanupSettings
description: Definieren Sie die Regel aus, wenn der Administrator die Geräte bereinigt werden möchte.
ms.openlocfilehash: f7782ac9d6571b58c8ed1e7964637736fcb5f3d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062171"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="f3cb2-103">Ressourcentyp managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="f3cb2-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="f3cb2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f3cb2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3cb2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f3cb2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3cb2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f3cb2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3cb2-107">Definieren Sie die Regel aus, wenn der Administrator die Geräte bereinigt werden möchte.</span><span class="sxs-lookup"><span data-stu-id="f3cb2-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="f3cb2-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f3cb2-108">Properties</span></span>
|<span data-ttu-id="f3cb2-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f3cb2-109">Property</span></span>|<span data-ttu-id="f3cb2-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f3cb2-110">Type</span></span>|<span data-ttu-id="f3cb2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f3cb2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3cb2-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="f3cb2-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="f3cb2-113">String</span><span class="sxs-lookup"><span data-stu-id="f3cb2-113">String</span></span>|<span data-ttu-id="f3cb2-114">Anzahl der Tage, wenn das Gerät nicht Intune kontaktiert hat.</span><span class="sxs-lookup"><span data-stu-id="f3cb2-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3cb2-115">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f3cb2-115">Relationships</span></span>
<span data-ttu-id="f3cb2-116">Keine</span><span class="sxs-lookup"><span data-stu-id="f3cb2-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f3cb2-117">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f3cb2-117">JSON Representation</span></span>
<span data-ttu-id="f3cb2-118">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f3cb2-118">Here is a JSON representation of the resource.</span></span>
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





