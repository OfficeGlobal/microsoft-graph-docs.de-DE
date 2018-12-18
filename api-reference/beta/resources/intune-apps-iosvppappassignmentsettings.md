---
title: iosVppAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.
author: tfitzmac
ms.openlocfilehash: 9e1233c9d5a33876da64ab3c75419c322ee83931
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321329"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="3b640-103">iosVppAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3b640-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="3b640-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b640-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b640-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b640-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b640-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3b640-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b640-107">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-VPP-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="3b640-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="3b640-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="3b640-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3b640-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3b640-109">Properties</span></span>
|<span data-ttu-id="3b640-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b640-110">Property</span></span>|<span data-ttu-id="3b640-111">Typ</span><span class="sxs-lookup"><span data-stu-id="3b640-111">Type</span></span>|<span data-ttu-id="3b640-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b640-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b640-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="3b640-113">useDeviceLicensing</span></span>|<span data-ttu-id="3b640-114">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="3b640-114">Boolean</span></span>|<span data-ttu-id="3b640-115">Gibt an, ob die Gerätelizenzierung verwendet werden soll oder nicht.</span><span class="sxs-lookup"><span data-stu-id="3b640-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="3b640-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="3b640-116">vpnConfigurationId</span></span>|<span data-ttu-id="3b640-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b640-117">String</span></span>|<span data-ttu-id="3b640-118">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="3b640-118">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b640-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3b640-119">Relationships</span></span>
<span data-ttu-id="3b640-120">Keine</span><span class="sxs-lookup"><span data-stu-id="3b640-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3b640-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3b640-121">JSON Representation</span></span>
<span data-ttu-id="3b640-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3b640-122">Here is a JSON representation of the resource.</span></span>
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





