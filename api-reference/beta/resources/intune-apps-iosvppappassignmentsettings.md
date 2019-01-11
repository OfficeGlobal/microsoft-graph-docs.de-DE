---
title: iosVppAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2dd3f8816aaa4e08066e329e4a9f4630e3f27f1d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867767"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="8c986-103">iosVppAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8c986-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="8c986-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8c986-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c986-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8c986-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c986-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8c986-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c986-107">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="8c986-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="8c986-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8c986-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c986-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8c986-109">Properties</span></span>
|<span data-ttu-id="8c986-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8c986-110">Property</span></span>|<span data-ttu-id="8c986-111">Typ</span><span class="sxs-lookup"><span data-stu-id="8c986-111">Type</span></span>|<span data-ttu-id="8c986-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8c986-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c986-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="8c986-113">useDeviceLicensing</span></span>|<span data-ttu-id="8c986-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="8c986-114">Boolean</span></span>|<span data-ttu-id="8c986-115">Gibt an, ob die Gerätelizenzierung verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="8c986-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="8c986-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="8c986-116">vpnConfigurationId</span></span>|<span data-ttu-id="8c986-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8c986-117">String</span></span>|<span data-ttu-id="8c986-118">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="8c986-118">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c986-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8c986-119">Relationships</span></span>
<span data-ttu-id="8c986-120">Keine</span><span class="sxs-lookup"><span data-stu-id="8c986-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c986-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8c986-121">JSON Representation</span></span>
<span data-ttu-id="8c986-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8c986-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```





