---
title: windowsKioskAzureADGroup-Ressourcentyp
description: Die Klasse, die zum Identifizieren einer AzureAD-Gruppe für die Kiosk Konfiguration verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f05bf9d01e8442a54c9fa70b863e3789309bd9d4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175136"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="61281-103">windowsKioskAzureADGroup-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="61281-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="61281-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="61281-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61281-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="61281-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61281-106">Die Klasse, die zum Identifizieren einer AzureAD-Gruppe für die Kiosk Konfiguration verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="61281-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="61281-107">Erbt von [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="61281-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="61281-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="61281-108">Properties</span></span>
|<span data-ttu-id="61281-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="61281-109">Property</span></span>|<span data-ttu-id="61281-110">Typ</span><span class="sxs-lookup"><span data-stu-id="61281-110">Type</span></span>|<span data-ttu-id="61281-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="61281-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61281-112">displayName</span><span class="sxs-lookup"><span data-stu-id="61281-112">displayName</span></span>|<span data-ttu-id="61281-113">String</span><span class="sxs-lookup"><span data-stu-id="61281-113">String</span></span>|<span data-ttu-id="61281-114">Der Anzeigename der AzureAD-Gruppe, die für diese Kiosk Konfiguration gesperrt wird.</span><span class="sxs-lookup"><span data-stu-id="61281-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="61281-115">groupId</span><span class="sxs-lookup"><span data-stu-id="61281-115">groupId</span></span>|<span data-ttu-id="61281-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="61281-116">String</span></span>|<span data-ttu-id="61281-117">Die ID der AzureAD-Gruppe, die für diese Kiosk Konfiguration gesperrt wird.</span><span class="sxs-lookup"><span data-stu-id="61281-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="61281-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="61281-118">Relationships</span></span>
<span data-ttu-id="61281-119">Keine</span><span class="sxs-lookup"><span data-stu-id="61281-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61281-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="61281-120">JSON Representation</span></span>
<span data-ttu-id="61281-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="61281-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```




