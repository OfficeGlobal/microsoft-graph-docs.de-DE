---
title: Ressourcentyp windowsUniversalAppXAppAssignmentSettings
description: Enthält Eigenschaften verwendet, wenn eine universelle AppX Windows mobile app zu einer Gruppe zuweisen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27755a483be44584aeb82166f56e825df79f8eaa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400718"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="6aba5-103">Ressourcentyp windowsUniversalAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6aba5-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="6aba5-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="6aba5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6aba5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6aba5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6aba5-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6aba5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aba5-107">Enthält Eigenschaften verwendet, wenn eine universelle AppX Windows mobile app zu einer Gruppe zuweisen.</span><span class="sxs-lookup"><span data-stu-id="6aba5-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="6aba5-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6aba5-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6aba5-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6aba5-109">Properties</span></span>
|<span data-ttu-id="6aba5-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6aba5-110">Property</span></span>|<span data-ttu-id="6aba5-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6aba5-111">Type</span></span>|<span data-ttu-id="6aba5-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6aba5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aba5-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="6aba5-113">useDeviceContext</span></span>|<span data-ttu-id="6aba5-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="6aba5-114">Boolean</span></span>|<span data-ttu-id="6aba5-115">Ob Ausführungskontexts Gerät für universelle AppX Windows mobile app verwenden.</span><span class="sxs-lookup"><span data-stu-id="6aba5-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6aba5-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6aba5-116">Relationships</span></span>
<span data-ttu-id="6aba5-117">Keine</span><span class="sxs-lookup"><span data-stu-id="6aba5-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6aba5-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6aba5-118">JSON Representation</span></span>
<span data-ttu-id="6aba5-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6aba5-119">Here is a JSON representation of the resource.</span></span>
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




