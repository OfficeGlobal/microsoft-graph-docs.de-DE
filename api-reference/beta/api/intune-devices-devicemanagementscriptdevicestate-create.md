---
title: Erstellen von deviceManagementScriptDeviceState
description: Erstellen eines neuen DeviceManagementScriptDeviceState-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3fbf8d69f7d421407b239a9265f51156a97bd6aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412863"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="50be4-103">Erstellen von deviceManagementScriptDeviceState</span><span class="sxs-lookup"><span data-stu-id="50be4-103">Create deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="50be4-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="50be4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="50be4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50be4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50be4-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="50be4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50be4-107">Erstellen eines neuen [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="50be4-107">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50be4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="50be4-108">Prerequisites</span></span>
<span data-ttu-id="50be4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="50be4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="50be4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="50be4-111">Permission type</span></span>|<span data-ttu-id="50be4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="50be4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50be4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="50be4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50be4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50be4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="50be4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="50be4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50be4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50be4-116">Not supported.</span></span>|
|<span data-ttu-id="50be4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="50be4-117">Application</span></span>|<span data-ttu-id="50be4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="50be4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50be4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="50be4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="50be4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="50be4-120">Request headers</span></span>
|<span data-ttu-id="50be4-121">Header</span><span class="sxs-lookup"><span data-stu-id="50be4-121">Header</span></span>|<span data-ttu-id="50be4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="50be4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50be4-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="50be4-123">Authorization</span></span>|<span data-ttu-id="50be4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="50be4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50be4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="50be4-125">Accept</span></span>|<span data-ttu-id="50be4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50be4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50be4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="50be4-127">Request body</span></span>
<span data-ttu-id="50be4-128">Geben Sie im Textkörper Anforderung für das Objekt DeviceManagementScriptDeviceState eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="50be4-128">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="50be4-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DeviceManagementScriptDeviceState erstellen.</span><span class="sxs-lookup"><span data-stu-id="50be4-129">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="50be4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50be4-130">Property</span></span>|<span data-ttu-id="50be4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="50be4-131">Type</span></span>|<span data-ttu-id="50be4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50be4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50be4-133">id</span><span class="sxs-lookup"><span data-stu-id="50be4-133">id</span></span>|<span data-ttu-id="50be4-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50be4-134">String</span></span>|<span data-ttu-id="50be4-135">Taste der Gerät Management Skript Gerät Zustand Entität.</span><span class="sxs-lookup"><span data-stu-id="50be4-135">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="50be4-136">runState</span><span class="sxs-lookup"><span data-stu-id="50be4-136">runState</span></span>|[<span data-ttu-id="50be4-137">runState</span><span class="sxs-lookup"><span data-stu-id="50be4-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="50be4-138">Status der letzten Ausführung des Skripts Management Gerät.</span><span class="sxs-lookup"><span data-stu-id="50be4-138">State of latest run of the device management script.</span></span> <span data-ttu-id="50be4-139">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="50be4-139">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="50be4-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="50be4-140">resultMessage</span></span>|<span data-ttu-id="50be4-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50be4-141">String</span></span>|<span data-ttu-id="50be4-142">Details der Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="50be4-142">Details of execution output.</span></span>|
|<span data-ttu-id="50be4-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="50be4-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="50be4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50be4-144">DateTimeOffset</span></span>|<span data-ttu-id="50be4-145">Zeitpunkt führt das Gerät Management-Skript aus.</span><span class="sxs-lookup"><span data-stu-id="50be4-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="50be4-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="50be4-146">errorCode</span></span>|<span data-ttu-id="50be4-147">Int32</span><span class="sxs-lookup"><span data-stu-id="50be4-147">Int32</span></span>|<span data-ttu-id="50be4-148">Fehlercode, fehlerhafte Ausführung des Skripts Management Gerät entspricht.</span><span class="sxs-lookup"><span data-stu-id="50be4-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="50be4-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="50be4-149">errorDescription</span></span>|<span data-ttu-id="50be4-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50be4-150">String</span></span>|<span data-ttu-id="50be4-151">Fehlerhafte Ausführung des Skripts Management Gerät entsprechend der Beschreibung des Fehlers.</span><span class="sxs-lookup"><span data-stu-id="50be4-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="50be4-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="50be4-152">Response</span></span>
<span data-ttu-id="50be4-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="50be4-153">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50be4-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="50be4-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="50be4-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="50be4-155">Request</span></span>
<span data-ttu-id="50be4-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="50be4-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="50be4-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="50be4-157">Response</span></span>
<span data-ttu-id="50be4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="50be4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




