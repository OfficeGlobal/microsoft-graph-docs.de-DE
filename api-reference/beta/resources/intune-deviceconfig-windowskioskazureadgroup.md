---
title: Ressourcentyp windowsKioskAzureADGroup
description: Die Klasse verwendet, um eine Gruppe AzureAD für die Konfiguration Kiosk identifizieren
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d4c8e0867346253c6501ebe8be490ba56800ab3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392570"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="81b10-103">Ressourcentyp windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="81b10-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="81b10-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="81b10-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="81b10-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="81b10-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81b10-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="81b10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81b10-107">Die Klasse verwendet, um eine Gruppe AzureAD für die Konfiguration Kiosk identifizieren</span><span class="sxs-lookup"><span data-stu-id="81b10-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="81b10-108">Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="81b10-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81b10-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="81b10-109">Properties</span></span>
|<span data-ttu-id="81b10-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="81b10-110">Property</span></span>|<span data-ttu-id="81b10-111">Typ</span><span class="sxs-lookup"><span data-stu-id="81b10-111">Type</span></span>|<span data-ttu-id="81b10-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="81b10-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81b10-113">displayName</span><span class="sxs-lookup"><span data-stu-id="81b10-113">displayName</span></span>|<span data-ttu-id="81b10-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81b10-114">String</span></span>|<span data-ttu-id="81b10-115">Der Anzeigename der Gruppe der AzureAD, die mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="81b10-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="81b10-116">groupId</span><span class="sxs-lookup"><span data-stu-id="81b10-116">groupId</span></span>|<span data-ttu-id="81b10-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="81b10-117">String</span></span>|<span data-ttu-id="81b10-118">Die ID der AzureAD Gruppe, die mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="81b10-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="81b10-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="81b10-119">Relationships</span></span>
<span data-ttu-id="81b10-120">Keine</span><span class="sxs-lookup"><span data-stu-id="81b10-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81b10-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="81b10-121">JSON Representation</span></span>
<span data-ttu-id="81b10-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="81b10-122">Here is a JSON representation of the resource.</span></span>
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




