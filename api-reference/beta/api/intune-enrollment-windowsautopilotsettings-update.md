---
title: WindowsAutopilotSettings aktualisieren
description: Aktualisieren der Eigenschaften eines windowsAutopilotSettings-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e479fece08101d290505c3156aee7c045c581328
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971864"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="280a0-103">WindowsAutopilotSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="280a0-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="280a0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="280a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="280a0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="280a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="280a0-106">Aktualisieren der Eigenschaften eines [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="280a0-106">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="280a0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="280a0-107">Prerequisites</span></span>
<span data-ttu-id="280a0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="280a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="280a0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="280a0-110">Permission type</span></span>|<span data-ttu-id="280a0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="280a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="280a0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="280a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="280a0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="280a0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="280a0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="280a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="280a0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="280a0-115">Not supported.</span></span>|
|<span data-ttu-id="280a0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="280a0-116">Application</span></span>|<span data-ttu-id="280a0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="280a0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="280a0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="280a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="280a0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="280a0-119">Request headers</span></span>
|<span data-ttu-id="280a0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="280a0-120">Header</span></span>|<span data-ttu-id="280a0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="280a0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="280a0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="280a0-122">Authorization</span></span>|<span data-ttu-id="280a0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="280a0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="280a0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="280a0-124">Accept</span></span>|<span data-ttu-id="280a0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="280a0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="280a0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="280a0-126">Request body</span></span>
<span data-ttu-id="280a0-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="280a0-127">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="280a0-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="280a0-128">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="280a0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="280a0-129">Property</span></span>|<span data-ttu-id="280a0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="280a0-130">Type</span></span>|<span data-ttu-id="280a0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="280a0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="280a0-132">id</span><span class="sxs-lookup"><span data-stu-id="280a0-132">id</span></span>|<span data-ttu-id="280a0-133">String</span><span class="sxs-lookup"><span data-stu-id="280a0-133">String</span></span>|<span data-ttu-id="280a0-134">GUID des Objekts</span><span class="sxs-lookup"><span data-stu-id="280a0-134">The GUID for the object</span></span>|
|<span data-ttu-id="280a0-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="280a0-135">lastSyncDateTime</span></span>|<span data-ttu-id="280a0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="280a0-136">DateTimeOffset</span></span>|<span data-ttu-id="280a0-137">Datum und Uhrzeit der letzten Datensynchronisierung mit dem DDS-Dienst.</span><span class="sxs-lookup"><span data-stu-id="280a0-137">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="280a0-138">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="280a0-138">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="280a0-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="280a0-139">DateTimeOffset</span></span>|<span data-ttu-id="280a0-140">Datum und Uhrzeit der letzten Datensynchronisierung mit dem DDS-Dienst.</span><span class="sxs-lookup"><span data-stu-id="280a0-140">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="280a0-141">syncStatus</span><span class="sxs-lookup"><span data-stu-id="280a0-141">syncStatus</span></span>|[<span data-ttu-id="280a0-142">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="280a0-142">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="280a0-143">Gibt den Status der Synchronisierung mit Device Data Sync (DDS)-Dienst an.</span><span class="sxs-lookup"><span data-stu-id="280a0-143">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="280a0-144">Mögliche Werte sind: `unknown`, `inProgress`, `completed` und `failed`.</span><span class="sxs-lookup"><span data-stu-id="280a0-144">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="280a0-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="280a0-145">Response</span></span>
<span data-ttu-id="280a0-146">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="280a0-146">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="280a0-147">Beispiel</span><span class="sxs-lookup"><span data-stu-id="280a0-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="280a0-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="280a0-148">Request</span></span>
<span data-ttu-id="280a0-149">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="280a0-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="280a0-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="280a0-150">Response</span></span>
<span data-ttu-id="280a0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="280a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




