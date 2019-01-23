---
title: Ressourcentyp win32LobAppAssignmentSettings
description: Enthält Eigenschaften, die zum Zuweisen einer mobilen Win32 LOB-app zu einer Gruppe.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 215b5c7086c2336f80bc0b812a108fbe2e2c1740
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430051"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="56535-103">Ressourcentyp win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="56535-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="56535-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="56535-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="56535-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56535-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56535-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="56535-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56535-107">Enthält Eigenschaften, die zum Zuweisen einer mobilen Win32 LOB-app zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="56535-107">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="56535-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="56535-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56535-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="56535-109">Properties</span></span>
|<span data-ttu-id="56535-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56535-110">Property</span></span>|<span data-ttu-id="56535-111">Typ</span><span class="sxs-lookup"><span data-stu-id="56535-111">Type</span></span>|<span data-ttu-id="56535-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56535-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56535-113">Benachrichtigungen</span><span class="sxs-lookup"><span data-stu-id="56535-113">notifications</span></span>|[<span data-ttu-id="56535-114">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="56535-114">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="56535-115">Der Status der Benachrichtigung diese app-Zuordnung.</span><span class="sxs-lookup"><span data-stu-id="56535-115">The notification status this app assignment.</span></span> <span data-ttu-id="56535-116">Mögliche Werte sind: `showAll`, `showReboot` und `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="56535-116">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56535-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="56535-117">Relationships</span></span>
<span data-ttu-id="56535-118">Keine</span><span class="sxs-lookup"><span data-stu-id="56535-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56535-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="56535-119">JSON Representation</span></span>
<span data-ttu-id="56535-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="56535-120">Here is a JSON representation of the resource.</span></span>
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




