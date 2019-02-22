---
title: win32LobAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen Win32-LOB-APP zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e98688a10c126ee6597f8d244e4a605a2addeaee
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172177"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="c9514-103">win32LobAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c9514-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c9514-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9514-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9514-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c9514-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9514-106">Enthält Eigenschaften zum Zuweisen einer mobilen Win32-LOB-APP zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="c9514-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="c9514-107">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="c9514-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9514-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c9514-108">Properties</span></span>
|<span data-ttu-id="c9514-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9514-109">Property</span></span>|<span data-ttu-id="c9514-110">Typ</span><span class="sxs-lookup"><span data-stu-id="c9514-110">Type</span></span>|<span data-ttu-id="c9514-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9514-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9514-112">Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="c9514-112">notifications</span></span>|[<span data-ttu-id="c9514-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="c9514-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="c9514-114">Der Benachrichtigungsstatus dieser APP-Zuweisung.</span><span class="sxs-lookup"><span data-stu-id="c9514-114">The notification status this app assignment.</span></span> <span data-ttu-id="c9514-115">Mögliche Werte sind: `showAll`, `showReboot` und `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="c9514-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9514-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c9514-116">Relationships</span></span>
<span data-ttu-id="c9514-117">Keine</span><span class="sxs-lookup"><span data-stu-id="c9514-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9514-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c9514-118">JSON Representation</span></span>
<span data-ttu-id="c9514-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c9514-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String"
}
```




