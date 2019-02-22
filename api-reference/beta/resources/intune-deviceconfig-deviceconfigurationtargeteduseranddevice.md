---
title: deviceConfigurationTargetedUserAndDevice-Ressourcentyp
description: Konflikt Zusammenfassung für eine Reihe von Geräte Konfigurationsrichtlinien.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48d73a532f08b0effb6581373300728ad21c5b37
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144142"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="3d4c1-103">deviceConfigurationTargetedUserAndDevice-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3d4c1-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="3d4c1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3d4c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d4c1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3d4c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d4c1-106">Konflikt Zusammenfassung für eine Reihe von Geräte Konfigurationsrichtlinien.</span><span class="sxs-lookup"><span data-stu-id="3d4c1-106">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="3d4c1-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3d4c1-107">Properties</span></span>
|<span data-ttu-id="3d4c1-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3d4c1-108">Property</span></span>|<span data-ttu-id="3d4c1-109">Typ</span><span class="sxs-lookup"><span data-stu-id="3d4c1-109">Type</span></span>|<span data-ttu-id="3d4c1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3d4c1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d4c1-111">deviceId</span><span class="sxs-lookup"><span data-stu-id="3d4c1-111">deviceId</span></span>|<span data-ttu-id="3d4c1-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d4c1-112">String</span></span>|<span data-ttu-id="3d4c1-113">Die ID des Geräts in der einchecken.</span><span class="sxs-lookup"><span data-stu-id="3d4c1-113">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="3d4c1-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="3d4c1-114">deviceName</span></span>|<span data-ttu-id="3d4c1-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d4c1-115">String</span></span>|<span data-ttu-id="3d4c1-116">Der Name des Geräts in der einchecken.</span><span class="sxs-lookup"><span data-stu-id="3d4c1-116">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="3d4c1-117">userId</span><span class="sxs-lookup"><span data-stu-id="3d4c1-117">userId</span></span>|<span data-ttu-id="3d4c1-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3d4c1-118">String</span></span>|<span data-ttu-id="3d4c1-119">Die ID des Benutzers in der einchecken.</span><span class="sxs-lookup"><span data-stu-id="3d4c1-119">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="3d4c1-120">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3d4c1-120">userDisplayName</span></span>|<span data-ttu-id="3d4c1-121">String</span><span class="sxs-lookup"><span data-stu-id="3d4c1-121">String</span></span>|<span data-ttu-id="3d4c1-122">Der Anzeigename des Benutzers in der Einchecken</span><span class="sxs-lookup"><span data-stu-id="3d4c1-122">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="3d4c1-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3d4c1-123">userPrincipalName</span></span>|<span data-ttu-id="3d4c1-124">String</span><span class="sxs-lookup"><span data-stu-id="3d4c1-124">String</span></span>|<span data-ttu-id="3d4c1-125">Der UPN des Benutzers beim Einchecken.</span><span class="sxs-lookup"><span data-stu-id="3d4c1-125">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="3d4c1-126">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="3d4c1-126">lastCheckinDateTime</span></span>|<span data-ttu-id="3d4c1-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d4c1-127">DateTimeOffset</span></span>|<span data-ttu-id="3d4c1-128">Letzter Eincheck Zeitpunkt für dieses Benutzer/Gerät-Paar.</span><span class="sxs-lookup"><span data-stu-id="3d4c1-128">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d4c1-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3d4c1-129">Relationships</span></span>
<span data-ttu-id="3d4c1-130">Keine</span><span class="sxs-lookup"><span data-stu-id="3d4c1-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d4c1-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3d4c1-131">JSON Representation</span></span>
<span data-ttu-id="3d4c1-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3d4c1-132">Here is a JSON representation of the resource.</span></span>
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




