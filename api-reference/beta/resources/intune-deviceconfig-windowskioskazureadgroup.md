---
title: Ressourcentyp windowsKioskAzureADGroup
description: Die Klasse verwendet, um eine Gruppe AzureAD für die Konfiguration Kiosk identifizieren
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 18ca386f0e1ee4647cff2a0ff5be9f2098d8f447
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964732"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="04318-103">Ressourcentyp windowsKioskAzureADGroup</span><span class="sxs-lookup"><span data-stu-id="04318-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="04318-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="04318-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04318-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="04318-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04318-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="04318-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04318-107">Die Klasse verwendet, um eine Gruppe AzureAD für die Konfiguration Kiosk identifizieren</span><span class="sxs-lookup"><span data-stu-id="04318-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>

<span data-ttu-id="04318-108">Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="04318-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="04318-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="04318-109">Properties</span></span>
|<span data-ttu-id="04318-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="04318-110">Property</span></span>|<span data-ttu-id="04318-111">Typ</span><span class="sxs-lookup"><span data-stu-id="04318-111">Type</span></span>|<span data-ttu-id="04318-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04318-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04318-113">displayName</span><span class="sxs-lookup"><span data-stu-id="04318-113">displayName</span></span>|<span data-ttu-id="04318-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04318-114">String</span></span>|<span data-ttu-id="04318-115">Der Anzeigename der Gruppe der AzureAD, die mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="04318-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="04318-116">groupId</span><span class="sxs-lookup"><span data-stu-id="04318-116">groupId</span></span>|<span data-ttu-id="04318-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="04318-117">String</span></span>|<span data-ttu-id="04318-118">Die ID der AzureAD Gruppe, die mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="04318-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="04318-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="04318-119">Relationships</span></span>
<span data-ttu-id="04318-120">Keine</span><span class="sxs-lookup"><span data-stu-id="04318-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04318-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="04318-121">JSON Representation</span></span>
<span data-ttu-id="04318-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="04318-122">Here is a JSON representation of the resource.</span></span>
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





