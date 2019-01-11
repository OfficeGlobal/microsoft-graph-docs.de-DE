---
title: Ressourcentyp windowsKioskAzureADUser
description: Die Klasse verwendet, um ein Benutzerkonto AzureAD für die Konfiguration Kiosk identifizieren
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 57b48bcdbac3f95da37704222cded29ba61cd32d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845885"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="46529-103">Ressourcentyp windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="46529-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="46529-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="46529-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46529-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46529-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46529-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="46529-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46529-107">Die Klasse verwendet, um ein Benutzerkonto AzureAD für die Konfiguration Kiosk identifizieren</span><span class="sxs-lookup"><span data-stu-id="46529-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>

<span data-ttu-id="46529-108">Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="46529-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="46529-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="46529-109">Properties</span></span>
|<span data-ttu-id="46529-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="46529-110">Property</span></span>|<span data-ttu-id="46529-111">Typ</span><span class="sxs-lookup"><span data-stu-id="46529-111">Type</span></span>|<span data-ttu-id="46529-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="46529-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46529-113">userId</span><span class="sxs-lookup"><span data-stu-id="46529-113">userId</span></span>|<span data-ttu-id="46529-114">String</span><span class="sxs-lookup"><span data-stu-id="46529-114">String</span></span>|<span data-ttu-id="46529-115">Die ID des Benutzers, die mit dieser Konfiguration Kiosk gesperrt werden AzureAD</span><span class="sxs-lookup"><span data-stu-id="46529-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="46529-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46529-116">userPrincipalName</span></span>|<span data-ttu-id="46529-117">String</span><span class="sxs-lookup"><span data-stu-id="46529-117">String</span></span>|<span data-ttu-id="46529-118">Die Benutzerkonten, die mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="46529-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="46529-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="46529-119">Relationships</span></span>
<span data-ttu-id="46529-120">Keine</span><span class="sxs-lookup"><span data-stu-id="46529-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="46529-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="46529-121">JSON Representation</span></span>
<span data-ttu-id="46529-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="46529-122">Here is a JSON representation of the resource.</span></span>
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





