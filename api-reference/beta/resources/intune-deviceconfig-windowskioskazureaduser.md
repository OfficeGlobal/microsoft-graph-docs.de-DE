---
title: Ressourcentyp windowsKioskAzureADUser
description: Die Klasse verwendet, um ein Benutzerkonto AzureAD für die Konfiguration Kiosk identifizieren
author: tfitzmac
ms.openlocfilehash: e4048b4cbea592af350af20bf433ca00ac6d4980
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330072"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="c3a68-103">Ressourcentyp windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="c3a68-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="c3a68-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c3a68-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3a68-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c3a68-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3a68-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c3a68-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3a68-107">Die Klasse verwendet, um ein Benutzerkonto AzureAD für die Konfiguration Kiosk identifizieren</span><span class="sxs-lookup"><span data-stu-id="c3a68-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>

<span data-ttu-id="c3a68-108">Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="c3a68-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c3a68-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c3a68-109">Properties</span></span>
|<span data-ttu-id="c3a68-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c3a68-110">Property</span></span>|<span data-ttu-id="c3a68-111">Typ</span><span class="sxs-lookup"><span data-stu-id="c3a68-111">Type</span></span>|<span data-ttu-id="c3a68-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3a68-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3a68-113">userId</span><span class="sxs-lookup"><span data-stu-id="c3a68-113">userId</span></span>|<span data-ttu-id="c3a68-114">String</span><span class="sxs-lookup"><span data-stu-id="c3a68-114">String</span></span>|<span data-ttu-id="c3a68-115">Die ID des Benutzers, die mit dieser Konfiguration Kiosk gesperrt werden AzureAD</span><span class="sxs-lookup"><span data-stu-id="c3a68-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="c3a68-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c3a68-116">userPrincipalName</span></span>|<span data-ttu-id="c3a68-117">String</span><span class="sxs-lookup"><span data-stu-id="c3a68-117">String</span></span>|<span data-ttu-id="c3a68-118">Die Benutzerkonten, die mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="c3a68-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3a68-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c3a68-119">Relationships</span></span>
<span data-ttu-id="c3a68-120">Keine</span><span class="sxs-lookup"><span data-stu-id="c3a68-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c3a68-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c3a68-121">JSON Representation</span></span>
<span data-ttu-id="c3a68-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c3a68-122">Here is a JSON representation of the resource.</span></span>
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





