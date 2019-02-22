---
title: windowsKioskAzureADUser-Ressourcentyp
description: Die Klasse, die zum Identifizieren eines AzureAD-Benutzerkontos für die Kiosk Konfiguration verwendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: feda393a6bee1b3cfc55d16cc91d321a5b99d54d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168250"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="e2925-103">windowsKioskAzureADUser-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e2925-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="e2925-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e2925-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2925-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e2925-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2925-106">Die Klasse, die zum Identifizieren eines AzureAD-Benutzerkontos für die Kiosk Konfiguration verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="e2925-106">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="e2925-107">Erbt von [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="e2925-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e2925-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e2925-108">Properties</span></span>
|<span data-ttu-id="e2925-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e2925-109">Property</span></span>|<span data-ttu-id="e2925-110">Typ</span><span class="sxs-lookup"><span data-stu-id="e2925-110">Type</span></span>|<span data-ttu-id="e2925-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2925-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2925-112">userId</span><span class="sxs-lookup"><span data-stu-id="e2925-112">userId</span></span>|<span data-ttu-id="e2925-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2925-113">String</span></span>|<span data-ttu-id="e2925-114">Die ID des AzureAD-Benutzers, der für diese Kiosk Konfiguration gesperrt wird.</span><span class="sxs-lookup"><span data-stu-id="e2925-114">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="e2925-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e2925-115">userPrincipalName</span></span>|<span data-ttu-id="e2925-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e2925-116">String</span></span>|<span data-ttu-id="e2925-117">Die Benutzerkonten, die für diese Kiosk Konfiguration gesperrt werden</span><span class="sxs-lookup"><span data-stu-id="e2925-117">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2925-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e2925-118">Relationships</span></span>
<span data-ttu-id="e2925-119">Keine</span><span class="sxs-lookup"><span data-stu-id="e2925-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2925-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e2925-120">JSON Representation</span></span>
<span data-ttu-id="e2925-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e2925-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```




