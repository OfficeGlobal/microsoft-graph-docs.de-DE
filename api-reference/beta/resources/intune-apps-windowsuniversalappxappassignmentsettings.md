---
title: Ressourcentyp windowsUniversalAppXAppAssignmentSettings
description: Enthält Eigenschaften verwendet, wenn eine universelle AppX Windows mobile app zu einer Gruppe zuweisen.
ms.openlocfilehash: 9694ab347be6edd1446df8aa7b46fb3652aee589
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062077"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="2abf4-103">Ressourcentyp windowsUniversalAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="2abf4-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="2abf4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2abf4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2abf4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2abf4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2abf4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2abf4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2abf4-107">Enthält Eigenschaften verwendet, wenn eine universelle AppX Windows mobile app zu einer Gruppe zuweisen.</span><span class="sxs-lookup"><span data-stu-id="2abf4-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>

<span data-ttu-id="2abf4-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2abf4-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2abf4-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2abf4-109">Properties</span></span>
|<span data-ttu-id="2abf4-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2abf4-110">Property</span></span>|<span data-ttu-id="2abf4-111">Typ</span><span class="sxs-lookup"><span data-stu-id="2abf4-111">Type</span></span>|<span data-ttu-id="2abf4-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2abf4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2abf4-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="2abf4-113">useDeviceContext</span></span>|<span data-ttu-id="2abf4-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2abf4-114">Boolean</span></span>|<span data-ttu-id="2abf4-115">Ob Ausführungskontexts Gerät für universelle AppX Windows mobile app verwenden.</span><span class="sxs-lookup"><span data-stu-id="2abf4-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2abf4-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="2abf4-116">Relationships</span></span>
<span data-ttu-id="2abf4-117">Keine</span><span class="sxs-lookup"><span data-stu-id="2abf4-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2abf4-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2abf4-118">JSON Representation</span></span>
<span data-ttu-id="2abf4-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2abf4-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```





