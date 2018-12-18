---
title: Ressourcentyp deviceConfigurationTargetedUserAndDevice
description: Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.
author: tfitzmac
ms.openlocfilehash: 04b0e31d0f3f099389e4901eb654139d286f4bd8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345241"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="4e300-103">Ressourcentyp deviceConfigurationTargetedUserAndDevice</span><span class="sxs-lookup"><span data-stu-id="4e300-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="4e300-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4e300-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e300-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e300-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e300-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4e300-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e300-107">Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.</span><span class="sxs-lookup"><span data-stu-id="4e300-107">Conflict summary for a set of device configuration policies.</span></span>
## <a name="properties"></a><span data-ttu-id="4e300-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4e300-108">Properties</span></span>
|<span data-ttu-id="4e300-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4e300-109">Property</span></span>|<span data-ttu-id="4e300-110">Typ</span><span class="sxs-lookup"><span data-stu-id="4e300-110">Type</span></span>|<span data-ttu-id="4e300-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4e300-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e300-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="4e300-112">deviceId</span></span>|<span data-ttu-id="4e300-113">String</span><span class="sxs-lookup"><span data-stu-id="4e300-113">String</span></span>|<span data-ttu-id="4e300-114">Die Id des Geräts in das Einchecken.</span><span class="sxs-lookup"><span data-stu-id="4e300-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="4e300-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="4e300-115">deviceName</span></span>|<span data-ttu-id="4e300-116">String</span><span class="sxs-lookup"><span data-stu-id="4e300-116">String</span></span>|<span data-ttu-id="4e300-117">Der Name des Geräts in das Einchecken.</span><span class="sxs-lookup"><span data-stu-id="4e300-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="4e300-118">userId</span><span class="sxs-lookup"><span data-stu-id="4e300-118">userId</span></span>|<span data-ttu-id="4e300-119">String</span><span class="sxs-lookup"><span data-stu-id="4e300-119">String</span></span>|<span data-ttu-id="4e300-120">Die Id des Benutzers in das Einchecken.</span><span class="sxs-lookup"><span data-stu-id="4e300-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="4e300-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4e300-121">userDisplayName</span></span>|<span data-ttu-id="4e300-122">String</span><span class="sxs-lookup"><span data-stu-id="4e300-122">String</span></span>|<span data-ttu-id="4e300-123">Der Anzeigename des Benutzers in das Einchecken</span><span class="sxs-lookup"><span data-stu-id="4e300-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="4e300-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4e300-124">userPrincipalName</span></span>|<span data-ttu-id="4e300-125">String</span><span class="sxs-lookup"><span data-stu-id="4e300-125">String</span></span>|<span data-ttu-id="4e300-126">Den UPN des Benutzers in das Einchecken.</span><span class="sxs-lookup"><span data-stu-id="4e300-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="4e300-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="4e300-127">lastCheckinDateTime</span></span>|<span data-ttu-id="4e300-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e300-128">DateTimeOffset</span></span>|<span data-ttu-id="4e300-129">Zeitpunkt der letzten Checkin für diese Benutzer/Geräte-Paar.</span><span class="sxs-lookup"><span data-stu-id="4e300-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e300-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4e300-130">Relationships</span></span>
<span data-ttu-id="4e300-131">Keine</span><span class="sxs-lookup"><span data-stu-id="4e300-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4e300-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4e300-132">JSON Representation</span></span>
<span data-ttu-id="4e300-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4e300-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```





