---
title: Erstellen von deviceManagementScriptDeviceState
description: Erstellen eines neuen DeviceManagementScriptDeviceState-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9663be4b0079763f8b0055bd68c9ccbc9c833fa5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963906"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="06adf-103">Erstellen von deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="06adf-103">Create deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="06adf-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="06adf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06adf-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06adf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06adf-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="06adf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06adf-107">Erstellen eines neuen [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="06adf-107">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06adf-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="06adf-108">Prerequisites</span></span>
<span data-ttu-id="06adf-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06adf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06adf-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06adf-111">Permission type</span></span>|<span data-ttu-id="06adf-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06adf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06adf-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06adf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="06adf-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06adf-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="06adf-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06adf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06adf-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06adf-116">Not supported.</span></span>|
|<span data-ttu-id="06adf-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06adf-117">Application</span></span>|<span data-ttu-id="06adf-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06adf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06adf-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06adf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="06adf-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06adf-120">Request headers</span></span>
|<span data-ttu-id="06adf-121">Header</span><span class="sxs-lookup"><span data-stu-id="06adf-121">Header</span></span>|<span data-ttu-id="06adf-122">Wert</span><span class="sxs-lookup"><span data-stu-id="06adf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06adf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06adf-123">Authorization</span></span>|<span data-ttu-id="06adf-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="06adf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06adf-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="06adf-125">Accept</span></span>|<span data-ttu-id="06adf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06adf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06adf-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06adf-127">Request body</span></span>
<span data-ttu-id="06adf-128">Geben Sie im Textkörper Anforderung für das Objekt DeviceManagementScriptDeviceState eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="06adf-128">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="06adf-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DeviceManagementScriptDeviceState erstellen.</span><span class="sxs-lookup"><span data-stu-id="06adf-129">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="06adf-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06adf-130">Property</span></span>|<span data-ttu-id="06adf-131">Typ</span><span class="sxs-lookup"><span data-stu-id="06adf-131">Type</span></span>|<span data-ttu-id="06adf-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06adf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06adf-133">id</span><span class="sxs-lookup"><span data-stu-id="06adf-133">id</span></span>|<span data-ttu-id="06adf-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06adf-134">String</span></span>|<span data-ttu-id="06adf-135">Taste der Gerät Management Skript Gerät Zustand Entität.</span><span class="sxs-lookup"><span data-stu-id="06adf-135">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="06adf-136">runState</span><span class="sxs-lookup"><span data-stu-id="06adf-136">runState</span></span>|[<span data-ttu-id="06adf-137">runState</span><span class="sxs-lookup"><span data-stu-id="06adf-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="06adf-138">Status der letzten Ausführung des Skripts Management Gerät.</span><span class="sxs-lookup"><span data-stu-id="06adf-138">State of latest run of the device management script.</span></span> <span data-ttu-id="06adf-139">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="06adf-139">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="06adf-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="06adf-140">resultMessage</span></span>|<span data-ttu-id="06adf-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06adf-141">String</span></span>|<span data-ttu-id="06adf-142">Details der Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="06adf-142">Details of execution output.</span></span>|
|<span data-ttu-id="06adf-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="06adf-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="06adf-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06adf-144">DateTimeOffset</span></span>|<span data-ttu-id="06adf-145">Zeitpunkt führt das Gerät Management-Skript aus.</span><span class="sxs-lookup"><span data-stu-id="06adf-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="06adf-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="06adf-146">errorCode</span></span>|<span data-ttu-id="06adf-147">Int32</span><span class="sxs-lookup"><span data-stu-id="06adf-147">Int32</span></span>|<span data-ttu-id="06adf-148">Fehlercode, fehlerhafte Ausführung des Skripts Management Gerät entspricht.</span><span class="sxs-lookup"><span data-stu-id="06adf-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="06adf-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="06adf-149">errorDescription</span></span>|<span data-ttu-id="06adf-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="06adf-150">String</span></span>|<span data-ttu-id="06adf-151">Fehlerhafte Ausführung des Skripts Management Gerät entsprechend der Beschreibung des Fehlers.</span><span class="sxs-lookup"><span data-stu-id="06adf-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="06adf-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="06adf-152">Response</span></span>
<span data-ttu-id="06adf-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="06adf-153">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06adf-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06adf-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="06adf-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06adf-155">Request</span></span>
<span data-ttu-id="06adf-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06adf-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="06adf-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="06adf-157">Response</span></span>
<span data-ttu-id="06adf-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06adf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





