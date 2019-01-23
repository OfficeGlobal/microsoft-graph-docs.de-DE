---
title: Ressourcentyp windowsKioskLocalGroup
description: Die Klasse verwendet, um eine lokale Gruppe für die Konfiguration Kiosk identifizieren
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1134b6a842b54dc49fcd15a92d21aef227b35182
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424630"
---
# <a name="windowskiosklocalgroup-resource-type"></a><span data-ttu-id="a6784-103">Ressourcentyp windowsKioskLocalGroup</span><span class="sxs-lookup"><span data-stu-id="a6784-103">windowsKioskLocalGroup resource type</span></span>

> <span data-ttu-id="a6784-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a6784-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a6784-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6784-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6784-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a6784-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6784-107">Die Klasse verwendet, um eine lokale Gruppe für die Konfiguration Kiosk identifizieren</span><span class="sxs-lookup"><span data-stu-id="a6784-107">The class used to identify a local group for the kiosk configuration</span></span>


<span data-ttu-id="a6784-108">Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="a6784-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a6784-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a6784-109">Properties</span></span>
|<span data-ttu-id="a6784-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a6784-110">Property</span></span>|<span data-ttu-id="a6784-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a6784-111">Type</span></span>|<span data-ttu-id="a6784-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6784-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6784-113">groupName</span><span class="sxs-lookup"><span data-stu-id="a6784-113">groupName</span></span>|<span data-ttu-id="a6784-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a6784-114">String</span></span>|<span data-ttu-id="a6784-115">Der Name der lokalen Gruppe, die mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="a6784-115">The name of the local group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6784-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a6784-116">Relationships</span></span>
<span data-ttu-id="a6784-117">Keine</span><span class="sxs-lookup"><span data-stu-id="a6784-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6784-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a6784-118">JSON Representation</span></span>
<span data-ttu-id="a6784-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a6784-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalGroup",
  "groupName": "String"
}
```




