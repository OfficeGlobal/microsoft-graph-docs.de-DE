---
title: iosStoreAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Store-App zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ca558a4c4be65a7ab8bd3aa880d39689a25863d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943526"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="27898-103">iosStoreAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="27898-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="27898-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="27898-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27898-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="27898-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27898-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="27898-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27898-107">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Store-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="27898-107">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="27898-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="27898-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="27898-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="27898-109">Properties</span></span>
|<span data-ttu-id="27898-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27898-110">Property</span></span>|<span data-ttu-id="27898-111">Typ</span><span class="sxs-lookup"><span data-stu-id="27898-111">Type</span></span>|<span data-ttu-id="27898-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27898-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27898-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="27898-113">vpnConfigurationId</span></span>|<span data-ttu-id="27898-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="27898-114">String</span></span>|<span data-ttu-id="27898-115">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="27898-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27898-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="27898-116">Relationships</span></span>
<span data-ttu-id="27898-117">Keine</span><span class="sxs-lookup"><span data-stu-id="27898-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="27898-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="27898-118">JSON Representation</span></span>
<span data-ttu-id="27898-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="27898-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```





