---
title: iosStoreAppAssignmentSettings-Ressourcentyp
description: Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Store-App zu einer Gruppe.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34a57d5aee554ddd47c0df863ff7fff373a7251a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408026"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="83231-103">iosStoreAppAssignmentSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="83231-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="83231-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="83231-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="83231-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="83231-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83231-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="83231-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83231-107">Enthält Eigenschaften zum Zuweisen einer mobilen iOS-Store-App zu einer Gruppe.</span><span class="sxs-lookup"><span data-stu-id="83231-107">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="83231-108">Erbt von [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="83231-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="83231-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="83231-109">Properties</span></span>
|<span data-ttu-id="83231-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="83231-110">Property</span></span>|<span data-ttu-id="83231-111">Typ</span><span class="sxs-lookup"><span data-stu-id="83231-111">Type</span></span>|<span data-ttu-id="83231-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="83231-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83231-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="83231-113">vpnConfigurationId</span></span>|<span data-ttu-id="83231-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="83231-114">String</span></span>|<span data-ttu-id="83231-115">Die VPN-Konfigurations-ID, die für diese App verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="83231-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83231-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="83231-116">Relationships</span></span>
<span data-ttu-id="83231-117">Keine</span><span class="sxs-lookup"><span data-stu-id="83231-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83231-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="83231-118">JSON Representation</span></span>
<span data-ttu-id="83231-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="83231-119">Here is a JSON representation of the resource.</span></span>
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




