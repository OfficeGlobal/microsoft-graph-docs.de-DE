---
title: Ressourcentyp deviceConfigurationTargetedUserAndDevice
description: Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e246d9731f5ed9d2ea888ba2b53d335fcbca19f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410742"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="da728-103">Ressourcentyp deviceConfigurationTargetedUserAndDevice</span><span class="sxs-lookup"><span data-stu-id="da728-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="da728-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="da728-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da728-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da728-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da728-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="da728-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da728-107">Zusammenfassung für einen Satz von Richtlinien für die Konfiguration von Geräte Konflikt.</span><span class="sxs-lookup"><span data-stu-id="da728-107">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="da728-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="da728-108">Properties</span></span>
|<span data-ttu-id="da728-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da728-109">Property</span></span>|<span data-ttu-id="da728-110">Typ</span><span class="sxs-lookup"><span data-stu-id="da728-110">Type</span></span>|<span data-ttu-id="da728-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da728-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da728-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="da728-112">deviceId</span></span>|<span data-ttu-id="da728-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da728-113">String</span></span>|<span data-ttu-id="da728-114">Die Id des Geräts in das Einchecken.</span><span class="sxs-lookup"><span data-stu-id="da728-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="da728-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="da728-115">deviceName</span></span>|<span data-ttu-id="da728-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da728-116">String</span></span>|<span data-ttu-id="da728-117">Der Name des Geräts in das Einchecken.</span><span class="sxs-lookup"><span data-stu-id="da728-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="da728-118">userId</span><span class="sxs-lookup"><span data-stu-id="da728-118">userId</span></span>|<span data-ttu-id="da728-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da728-119">String</span></span>|<span data-ttu-id="da728-120">Die Id des Benutzers in das Einchecken.</span><span class="sxs-lookup"><span data-stu-id="da728-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="da728-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="da728-121">userDisplayName</span></span>|<span data-ttu-id="da728-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da728-122">String</span></span>|<span data-ttu-id="da728-123">Der Anzeigename des Benutzers in das Einchecken</span><span class="sxs-lookup"><span data-stu-id="da728-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="da728-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="da728-124">userPrincipalName</span></span>|<span data-ttu-id="da728-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da728-125">String</span></span>|<span data-ttu-id="da728-126">Den UPN des Benutzers in das Einchecken.</span><span class="sxs-lookup"><span data-stu-id="da728-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="da728-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="da728-127">lastCheckinDateTime</span></span>|<span data-ttu-id="da728-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da728-128">DateTimeOffset</span></span>|<span data-ttu-id="da728-129">Zeitpunkt der letzten Checkin für diese Benutzer/Geräte-Paar.</span><span class="sxs-lookup"><span data-stu-id="da728-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da728-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="da728-130">Relationships</span></span>
<span data-ttu-id="da728-131">Keine</span><span class="sxs-lookup"><span data-stu-id="da728-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da728-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="da728-132">JSON Representation</span></span>
<span data-ttu-id="da728-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="da728-133">Here is a JSON representation of the resource.</span></span>
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




