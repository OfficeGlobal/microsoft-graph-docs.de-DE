---
title: windowsAutopilotSettings-Ressourcentyp
description: Die windowsAutopilotSettings-Ressource stellt ein Windows Autopilot-Konto zum Synchronisieren von Daten mit dem Windows-Gerätedaten-Synchronisierungsdienst dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b34d6edbed5bc98989ea70186b081d5c88a1c1b6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140516"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="f138a-103">windowsAutopilotSettings-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f138a-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="f138a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f138a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f138a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f138a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f138a-106">Die windowsAutopilotSettings-Ressource stellt ein Windows Autopilot-Konto zum Synchronisieren von Daten mit dem Windows-Gerätedaten-Synchronisierungsdienst dar.</span><span class="sxs-lookup"><span data-stu-id="f138a-106">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="f138a-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="f138a-107">Methods</span></span>
|<span data-ttu-id="f138a-108">Methode</span><span class="sxs-lookup"><span data-stu-id="f138a-108">Method</span></span>|<span data-ttu-id="f138a-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="f138a-109">Return Type</span></span>|<span data-ttu-id="f138a-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f138a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f138a-111">WindowsAutopilotSettings abrufen</span><span class="sxs-lookup"><span data-stu-id="f138a-111">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="f138a-112">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="f138a-112">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="f138a-113">Lesen von Eigenschaften und Beziehungen des [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f138a-113">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="f138a-114">WindowsAutopilotSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="f138a-114">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="f138a-115">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="f138a-115">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="f138a-116">Aktualisieren der Eigenschaften eines [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f138a-116">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="f138a-117">sync-Aktion</span><span class="sxs-lookup"><span data-stu-id="f138a-117">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="f138a-118">Keine</span><span class="sxs-lookup"><span data-stu-id="f138a-118">None</span></span>|<span data-ttu-id="f138a-119">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="f138a-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f138a-120">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f138a-120">Properties</span></span>
|<span data-ttu-id="f138a-121">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f138a-121">Property</span></span>|<span data-ttu-id="f138a-122">Typ</span><span class="sxs-lookup"><span data-stu-id="f138a-122">Type</span></span>|<span data-ttu-id="f138a-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f138a-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f138a-124">id</span><span class="sxs-lookup"><span data-stu-id="f138a-124">id</span></span>|<span data-ttu-id="f138a-125">String</span><span class="sxs-lookup"><span data-stu-id="f138a-125">String</span></span>|<span data-ttu-id="f138a-126">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="f138a-126">The GUID for the object</span></span>|
|<span data-ttu-id="f138a-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f138a-127">lastSyncDateTime</span></span>|<span data-ttu-id="f138a-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f138a-128">DateTimeOffset</span></span>|<span data-ttu-id="f138a-129">Datum und Uhrzeit der letzten Datensynchronisierung mit dem DDS-Dienst.</span><span class="sxs-lookup"><span data-stu-id="f138a-129">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="f138a-130">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="f138a-130">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="f138a-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f138a-131">DateTimeOffset</span></span>|<span data-ttu-id="f138a-132">Datum und Uhrzeit der letzten Datensynchronisierung mit dem DDS-Dienst.</span><span class="sxs-lookup"><span data-stu-id="f138a-132">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="f138a-133">syncStatus</span><span class="sxs-lookup"><span data-stu-id="f138a-133">syncStatus</span></span>|[<span data-ttu-id="f138a-134">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="f138a-134">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="f138a-135">Gibt den Status der Synchronisierung mit Device Data Sync (DDS)-Dienst an.</span><span class="sxs-lookup"><span data-stu-id="f138a-135">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="f138a-136">Mögliche Werte: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="f138a-136">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f138a-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f138a-137">Relationships</span></span>
<span data-ttu-id="f138a-138">Keine</span><span class="sxs-lookup"><span data-stu-id="f138a-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f138a-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f138a-139">JSON Representation</span></span>
<span data-ttu-id="f138a-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f138a-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```




