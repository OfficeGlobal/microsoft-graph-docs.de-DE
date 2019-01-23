---
title: DeviceManagementScriptDeviceState aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceManagementScriptDeviceState-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35768793279cdb96494a26dac8854f74e3c267ad
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395153"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="948e7-103">DeviceManagementScriptDeviceState aktualisieren</span><span class="sxs-lookup"><span data-stu-id="948e7-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="948e7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="948e7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="948e7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="948e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="948e7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="948e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="948e7-107">Aktualisieren Sie die Eigenschaften eines [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="948e7-107">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="948e7-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="948e7-108">Prerequisites</span></span>
<span data-ttu-id="948e7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="948e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="948e7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="948e7-111">Permission type</span></span>|<span data-ttu-id="948e7-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="948e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="948e7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="948e7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="948e7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="948e7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="948e7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="948e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="948e7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="948e7-116">Not supported.</span></span>|
|<span data-ttu-id="948e7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="948e7-117">Application</span></span>|<span data-ttu-id="948e7-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="948e7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="948e7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="948e7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="948e7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="948e7-120">Request headers</span></span>
|<span data-ttu-id="948e7-121">Header</span><span class="sxs-lookup"><span data-stu-id="948e7-121">Header</span></span>|<span data-ttu-id="948e7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="948e7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="948e7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="948e7-123">Authorization</span></span>|<span data-ttu-id="948e7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="948e7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="948e7-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="948e7-125">Accept</span></span>|<span data-ttu-id="948e7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="948e7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="948e7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="948e7-127">Request body</span></span>
<span data-ttu-id="948e7-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="948e7-128">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="948e7-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="948e7-129">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="948e7-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="948e7-130">Property</span></span>|<span data-ttu-id="948e7-131">Typ</span><span class="sxs-lookup"><span data-stu-id="948e7-131">Type</span></span>|<span data-ttu-id="948e7-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="948e7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="948e7-133">id</span><span class="sxs-lookup"><span data-stu-id="948e7-133">id</span></span>|<span data-ttu-id="948e7-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="948e7-134">String</span></span>|<span data-ttu-id="948e7-135">Taste der Gerät Management Skript Gerät Zustand Entität.</span><span class="sxs-lookup"><span data-stu-id="948e7-135">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="948e7-136">runState</span><span class="sxs-lookup"><span data-stu-id="948e7-136">runState</span></span>|[<span data-ttu-id="948e7-137">runState</span><span class="sxs-lookup"><span data-stu-id="948e7-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="948e7-138">Status der letzten Ausführung des Skripts Management Gerät.</span><span class="sxs-lookup"><span data-stu-id="948e7-138">State of latest run of the device management script.</span></span> <span data-ttu-id="948e7-139">Mögliche Werte sind: `unknown`, `success` und `fail`.</span><span class="sxs-lookup"><span data-stu-id="948e7-139">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="948e7-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="948e7-140">resultMessage</span></span>|<span data-ttu-id="948e7-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="948e7-141">String</span></span>|<span data-ttu-id="948e7-142">Details der Ausgabe.</span><span class="sxs-lookup"><span data-stu-id="948e7-142">Details of execution output.</span></span>|
|<span data-ttu-id="948e7-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="948e7-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="948e7-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="948e7-144">DateTimeOffset</span></span>|<span data-ttu-id="948e7-145">Zeitpunkt führt das Gerät Management-Skript aus.</span><span class="sxs-lookup"><span data-stu-id="948e7-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="948e7-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="948e7-146">errorCode</span></span>|<span data-ttu-id="948e7-147">Int32</span><span class="sxs-lookup"><span data-stu-id="948e7-147">Int32</span></span>|<span data-ttu-id="948e7-148">Fehlercode, fehlerhafte Ausführung des Skripts Management Gerät entspricht.</span><span class="sxs-lookup"><span data-stu-id="948e7-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="948e7-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="948e7-149">errorDescription</span></span>|<span data-ttu-id="948e7-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="948e7-150">String</span></span>|<span data-ttu-id="948e7-151">Fehlerhafte Ausführung des Skripts Management Gerät entsprechend der Beschreibung des Fehlers.</span><span class="sxs-lookup"><span data-stu-id="948e7-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="948e7-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="948e7-152">Response</span></span>
<span data-ttu-id="948e7-153">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="948e7-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="948e7-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="948e7-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="948e7-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="948e7-155">Request</span></span>
<span data-ttu-id="948e7-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="948e7-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
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

### <a name="response"></a><span data-ttu-id="948e7-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="948e7-157">Response</span></span>
<span data-ttu-id="948e7-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="948e7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




