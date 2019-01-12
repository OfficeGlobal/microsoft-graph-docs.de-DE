---
title: Ressourcentyp windowsKioskAzureADUser
description: Die Klasse verwendet, um ein Benutzerkonto AzureAD für die Konfiguration Kiosk identifizieren
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4497c6d42db45f518e3ef93e78e50d25f473ac00
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984143"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="bda63-103">Ressourcentyp windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="bda63-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="bda63-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bda63-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bda63-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bda63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bda63-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bda63-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bda63-107">Die Klasse verwendet, um ein Benutzerkonto AzureAD für die Konfiguration Kiosk identifizieren</span><span class="sxs-lookup"><span data-stu-id="bda63-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>

<span data-ttu-id="bda63-108">Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="bda63-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bda63-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bda63-109">Properties</span></span>
|<span data-ttu-id="bda63-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bda63-110">Property</span></span>|<span data-ttu-id="bda63-111">Typ</span><span class="sxs-lookup"><span data-stu-id="bda63-111">Type</span></span>|<span data-ttu-id="bda63-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bda63-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bda63-113">userId</span><span class="sxs-lookup"><span data-stu-id="bda63-113">userId</span></span>|<span data-ttu-id="bda63-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bda63-114">String</span></span>|<span data-ttu-id="bda63-115">Die ID des Benutzers, die mit dieser Konfiguration Kiosk gesperrt werden AzureAD</span><span class="sxs-lookup"><span data-stu-id="bda63-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="bda63-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bda63-116">userPrincipalName</span></span>|<span data-ttu-id="bda63-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bda63-117">String</span></span>|<span data-ttu-id="bda63-118">Die Benutzerkonten, die mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="bda63-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="bda63-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bda63-119">Relationships</span></span>
<span data-ttu-id="bda63-120">Keine</span><span class="sxs-lookup"><span data-stu-id="bda63-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bda63-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bda63-121">JSON Representation</span></span>
<span data-ttu-id="bda63-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bda63-122">Here is a JSON representation of the resource.</span></span>
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





