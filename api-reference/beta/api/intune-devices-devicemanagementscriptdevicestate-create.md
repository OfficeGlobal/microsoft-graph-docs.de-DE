---
title: DeviceManagementScriptDeviceState erstellen
description: Erstellen eines neuen deviceManagementScriptDeviceState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93bd605b64b652346fbcba03e0fc2952ad6dfaa4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175080"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="19765-103">DeviceManagementScriptDeviceState erstellen</span><span class="sxs-lookup"><span data-stu-id="19765-103">Create deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="19765-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19765-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19765-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="19765-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19765-106">Erstellen eines neuen [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="19765-106">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19765-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="19765-107">Prerequisites</span></span>
<span data-ttu-id="19765-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="19765-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="19765-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19765-110">Permission type</span></span>|<span data-ttu-id="19765-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19765-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19765-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19765-112">Delegated (work or school account)</span></span>|<span data-ttu-id="19765-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19765-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="19765-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19765-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19765-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19765-115">Not supported.</span></span>|
|<span data-ttu-id="19765-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19765-116">Application</span></span>|<span data-ttu-id="19765-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19765-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19765-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19765-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="19765-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19765-119">Request headers</span></span>
|<span data-ttu-id="19765-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="19765-120">Header</span></span>|<span data-ttu-id="19765-121">Wert</span><span class="sxs-lookup"><span data-stu-id="19765-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19765-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="19765-122">Authorization</span></span>|<span data-ttu-id="19765-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="19765-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19765-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="19765-124">Accept</span></span>|<span data-ttu-id="19765-125">application/json</span><span class="sxs-lookup"><span data-stu-id="19765-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19765-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19765-126">Request body</span></span>
<span data-ttu-id="19765-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das deviceManagementScriptDeviceState-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="19765-127">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="19765-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der deviceManagementScriptDeviceState erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="19765-128">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="19765-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="19765-129">Property</span></span>|<span data-ttu-id="19765-130">Typ</span><span class="sxs-lookup"><span data-stu-id="19765-130">Type</span></span>|<span data-ttu-id="19765-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19765-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19765-132">id</span><span class="sxs-lookup"><span data-stu-id="19765-132">id</span></span>|<span data-ttu-id="19765-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19765-133">String</span></span>|<span data-ttu-id="19765-134">Schlüssel der Gerätestatus Entität des Device Management-Skripts.</span><span class="sxs-lookup"><span data-stu-id="19765-134">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="19765-135">runState</span><span class="sxs-lookup"><span data-stu-id="19765-135">runState</span></span>|[<span data-ttu-id="19765-136">runState</span><span class="sxs-lookup"><span data-stu-id="19765-136">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="19765-137">Status der letzten Ausführung des Geräteverwaltungs-Skripts.</span><span class="sxs-lookup"><span data-stu-id="19765-137">State of latest run of the device management script.</span></span> <span data-ttu-id="19765-138">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="19765-138">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="19765-139">resultMessage</span><span class="sxs-lookup"><span data-stu-id="19765-139">resultMessage</span></span>|<span data-ttu-id="19765-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19765-140">String</span></span>|<span data-ttu-id="19765-141">Details der Ausführungs Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="19765-141">Details of execution output.</span></span>|
|<span data-ttu-id="19765-142">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="19765-142">lastStateUpdateDateTime</span></span>|<span data-ttu-id="19765-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19765-143">DateTimeOffset</span></span>|<span data-ttu-id="19765-144">Der letzte Zeitpunkt, zu dem das Geräte Verwaltungsskript ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="19765-144">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="19765-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="19765-145">errorCode</span></span>|<span data-ttu-id="19765-146">Int32</span><span class="sxs-lookup"><span data-stu-id="19765-146">Int32</span></span>|<span data-ttu-id="19765-147">Fehlercode, der einer fehlerhaften Ausführung des Geräteverwaltungsskripts entspricht.</span><span class="sxs-lookup"><span data-stu-id="19765-147">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="19765-148">errorDescription</span><span class="sxs-lookup"><span data-stu-id="19765-148">errorDescription</span></span>|<span data-ttu-id="19765-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="19765-149">String</span></span>|<span data-ttu-id="19765-150">Fehlerbeschreibung, die dem fehlerhaften Ausführen des Geräteverwaltungsskripts entspricht.</span><span class="sxs-lookup"><span data-stu-id="19765-150">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="19765-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="19765-151">Response</span></span>
<span data-ttu-id="19765-152">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="19765-152">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19765-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="19765-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="19765-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19765-154">Request</span></span>
<span data-ttu-id="19765-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="19765-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```

### <a name="response"></a><span data-ttu-id="19765-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="19765-156">Response</span></span>
<span data-ttu-id="19765-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19765-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```




