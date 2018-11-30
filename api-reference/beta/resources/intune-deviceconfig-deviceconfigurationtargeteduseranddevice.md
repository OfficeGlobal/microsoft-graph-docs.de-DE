---
title: Ressourcentyp deviceConfigurationTargetedUserAndDevice
description: Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.
ms.openlocfilehash: 6f79a8fe24e06d2bdafa81c30cabf8158b4e5773
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058980"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="67d22-103">Ressourcentyp deviceConfigurationTargetedUserAndDevice</span><span class="sxs-lookup"><span data-stu-id="67d22-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="67d22-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="67d22-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67d22-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="67d22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67d22-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="67d22-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67d22-107">Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.</span><span class="sxs-lookup"><span data-stu-id="67d22-107">Conflict summary for a set of device configuration policies.</span></span>
## <a name="properties"></a><span data-ttu-id="67d22-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="67d22-108">Properties</span></span>
|<span data-ttu-id="67d22-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="67d22-109">Property</span></span>|<span data-ttu-id="67d22-110">Typ</span><span class="sxs-lookup"><span data-stu-id="67d22-110">Type</span></span>|<span data-ttu-id="67d22-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="67d22-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67d22-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="67d22-112">deviceId</span></span>|<span data-ttu-id="67d22-113">String</span><span class="sxs-lookup"><span data-stu-id="67d22-113">String</span></span>|<span data-ttu-id="67d22-114">Die Id des Geräts in das Einchecken.</span><span class="sxs-lookup"><span data-stu-id="67d22-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="67d22-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="67d22-115">deviceName</span></span>|<span data-ttu-id="67d22-116">String</span><span class="sxs-lookup"><span data-stu-id="67d22-116">String</span></span>|<span data-ttu-id="67d22-117">Der Name des Geräts in das Einchecken.</span><span class="sxs-lookup"><span data-stu-id="67d22-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="67d22-118">userId</span><span class="sxs-lookup"><span data-stu-id="67d22-118">userId</span></span>|<span data-ttu-id="67d22-119">String</span><span class="sxs-lookup"><span data-stu-id="67d22-119">String</span></span>|<span data-ttu-id="67d22-120">Die Id des Benutzers in das Einchecken.</span><span class="sxs-lookup"><span data-stu-id="67d22-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="67d22-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="67d22-121">userDisplayName</span></span>|<span data-ttu-id="67d22-122">String</span><span class="sxs-lookup"><span data-stu-id="67d22-122">String</span></span>|<span data-ttu-id="67d22-123">Der Anzeigename des Benutzers in das Einchecken</span><span class="sxs-lookup"><span data-stu-id="67d22-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="67d22-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="67d22-124">userPrincipalName</span></span>|<span data-ttu-id="67d22-125">String</span><span class="sxs-lookup"><span data-stu-id="67d22-125">String</span></span>|<span data-ttu-id="67d22-126">Den UPN des Benutzers in das Einchecken.</span><span class="sxs-lookup"><span data-stu-id="67d22-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="67d22-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="67d22-127">lastCheckinDateTime</span></span>|<span data-ttu-id="67d22-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67d22-128">DateTimeOffset</span></span>|<span data-ttu-id="67d22-129">Zeitpunkt der letzten Checkin für diese Benutzer/Geräte-Paar.</span><span class="sxs-lookup"><span data-stu-id="67d22-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67d22-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="67d22-130">Relationships</span></span>
<span data-ttu-id="67d22-131">Keine</span><span class="sxs-lookup"><span data-stu-id="67d22-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="67d22-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="67d22-132">JSON Representation</span></span>
<span data-ttu-id="67d22-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="67d22-133">Here is a JSON representation of the resource.</span></span>
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





