---
title: Ressourcentyp windowsAppXAppAssignmentSettings
description: Enthält Eigenschaften verwendet, wenn eine AppX Windows mobile app zu einer Gruppe zuweisen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2ee4079bcaf25802fe2e1ceac5bbba5eb47c8da4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854264"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="f1ef9-103">Ressourcentyp windowsAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="f1ef9-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="f1ef9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f1ef9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1ef9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1ef9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1ef9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f1ef9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1ef9-107">Enthält Eigenschaften verwendet, wenn eine AppX Windows mobile app zu einer Gruppe zuweisen.</span><span class="sxs-lookup"><span data-stu-id="f1ef9-107">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>

<span data-ttu-id="f1ef9-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f1ef9-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f1ef9-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f1ef9-109">Properties</span></span>
|<span data-ttu-id="f1ef9-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f1ef9-110">Property</span></span>|<span data-ttu-id="f1ef9-111">Typ</span><span class="sxs-lookup"><span data-stu-id="f1ef9-111">Type</span></span>|<span data-ttu-id="f1ef9-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f1ef9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1ef9-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="f1ef9-113">useDeviceContext</span></span>|<span data-ttu-id="f1ef9-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="f1ef9-114">Boolean</span></span>|<span data-ttu-id="f1ef9-115">Ob Ausführungskontexts Gerät für AppX Windows mobile app verwenden.</span><span class="sxs-lookup"><span data-stu-id="f1ef9-115">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1ef9-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f1ef9-116">Relationships</span></span>
<span data-ttu-id="f1ef9-117">Keine</span><span class="sxs-lookup"><span data-stu-id="f1ef9-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1ef9-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f1ef9-118">JSON Representation</span></span>
<span data-ttu-id="f1ef9-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f1ef9-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```





