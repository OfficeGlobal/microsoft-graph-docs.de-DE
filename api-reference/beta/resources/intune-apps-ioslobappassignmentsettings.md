---
title: iosLobAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f2e0c9ca5b2628343b79ff972e50c3684651c23
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990513"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="73566-103">iosLobAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="73566-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="73566-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="73566-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="73566-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="73566-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73566-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="73566-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73566-107">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="73566-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="73566-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="73566-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="73566-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="73566-109">Properties</span></span>
|<span data-ttu-id="73566-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73566-110">Property</span></span>|<span data-ttu-id="73566-111">Typ</span><span class="sxs-lookup"><span data-stu-id="73566-111">Type</span></span>|<span data-ttu-id="73566-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73566-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73566-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="73566-113">vpnConfigurationId</span></span>|<span data-ttu-id="73566-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73566-114">String</span></span>|<span data-ttu-id="73566-115">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="73566-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73566-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="73566-116">Relationships</span></span>
<span data-ttu-id="73566-117">Keine</span><span class="sxs-lookup"><span data-stu-id="73566-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="73566-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="73566-118">JSON Representation</span></span>
<span data-ttu-id="73566-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="73566-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```





