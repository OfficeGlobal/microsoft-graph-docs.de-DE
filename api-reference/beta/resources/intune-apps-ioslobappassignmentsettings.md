---
title: iosLobAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: db267df76db2171a869667e62e33d94644652ec8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882110"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="ce1e3-103">iosLobAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ce1e3-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="ce1e3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ce1e3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce1e3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ce1e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce1e3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ce1e3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce1e3-107">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Branchen-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="ce1e3-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="ce1e3-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ce1e3-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ce1e3-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ce1e3-109">Properties</span></span>
|<span data-ttu-id="ce1e3-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ce1e3-110">Property</span></span>|<span data-ttu-id="ce1e3-111">Typ</span><span class="sxs-lookup"><span data-stu-id="ce1e3-111">Type</span></span>|<span data-ttu-id="ce1e3-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ce1e3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce1e3-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="ce1e3-113">vpnConfigurationId</span></span>|<span data-ttu-id="ce1e3-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ce1e3-114">String</span></span>|<span data-ttu-id="ce1e3-115">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="ce1e3-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce1e3-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ce1e3-116">Relationships</span></span>
<span data-ttu-id="ce1e3-117">Keine</span><span class="sxs-lookup"><span data-stu-id="ce1e3-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ce1e3-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ce1e3-118">JSON Representation</span></span>
<span data-ttu-id="ce1e3-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ce1e3-119">Here is a JSON representation of the resource.</span></span>
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





