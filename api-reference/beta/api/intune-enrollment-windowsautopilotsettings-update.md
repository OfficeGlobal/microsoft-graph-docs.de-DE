---
title: WindowsAutopilotSettings aktualisieren
description: Aktualisieren der Eigenschaften eines windowsAutopilotSettings-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da2b5e622d9f5d8657e78162bff40d5843482081
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144121"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="e296d-103">WindowsAutopilotSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e296d-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="e296d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e296d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e296d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e296d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e296d-106">Aktualisieren der Eigenschaften eines [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e296d-106">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e296d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e296d-107">Prerequisites</span></span>
<span data-ttu-id="e296d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e296d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e296d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e296d-110">Permission type</span></span>|<span data-ttu-id="e296d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e296d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e296d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e296d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e296d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e296d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e296d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e296d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e296d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e296d-115">Not supported.</span></span>|
|<span data-ttu-id="e296d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e296d-116">Application</span></span>|<span data-ttu-id="e296d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e296d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e296d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e296d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="e296d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e296d-119">Request headers</span></span>
|<span data-ttu-id="e296d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e296d-120">Header</span></span>|<span data-ttu-id="e296d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e296d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e296d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e296d-122">Authorization</span></span>|<span data-ttu-id="e296d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e296d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e296d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e296d-124">Accept</span></span>|<span data-ttu-id="e296d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e296d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e296d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e296d-126">Request body</span></span>
<span data-ttu-id="e296d-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="e296d-127">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="e296d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e296d-128">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="e296d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e296d-129">Property</span></span>|<span data-ttu-id="e296d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e296d-130">Type</span></span>|<span data-ttu-id="e296d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e296d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e296d-132">id</span><span class="sxs-lookup"><span data-stu-id="e296d-132">id</span></span>|<span data-ttu-id="e296d-133">String</span><span class="sxs-lookup"><span data-stu-id="e296d-133">String</span></span>|<span data-ttu-id="e296d-134">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="e296d-134">The GUID for the object</span></span>|
|<span data-ttu-id="e296d-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e296d-135">lastSyncDateTime</span></span>|<span data-ttu-id="e296d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e296d-136">DateTimeOffset</span></span>|<span data-ttu-id="e296d-137">Datum und Uhrzeit der letzten Datensynchronisierung mit dem DDS-Dienst.</span><span class="sxs-lookup"><span data-stu-id="e296d-137">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="e296d-138">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="e296d-138">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="e296d-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e296d-139">DateTimeOffset</span></span>|<span data-ttu-id="e296d-140">Datum und Uhrzeit der letzten Datensynchronisierung mit dem DDS-Dienst.</span><span class="sxs-lookup"><span data-stu-id="e296d-140">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="e296d-141">syncStatus</span><span class="sxs-lookup"><span data-stu-id="e296d-141">syncStatus</span></span>|[<span data-ttu-id="e296d-142">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="e296d-142">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="e296d-143">Gibt den Status der Synchronisierung mit Device Data Sync (DDS)-Dienst an.</span><span class="sxs-lookup"><span data-stu-id="e296d-143">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="e296d-144">Mögliche Werte sind: `unknown`, `inProgress`, `completed` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="e296d-144">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="e296d-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="e296d-145">Response</span></span>
<span data-ttu-id="e296d-146">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e296d-146">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e296d-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e296d-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="e296d-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e296d-148">Request</span></span>
<span data-ttu-id="e296d-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e296d-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a><span data-ttu-id="e296d-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="e296d-150">Response</span></span>
<span data-ttu-id="e296d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e296d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "08c16770-6770-08c1-7067-c1087067c108",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```




