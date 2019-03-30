---
title: Aktualisieren von „deviceInstallState“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9866774b41c37a78604d1f4f0dfb6b87db36fdfd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986761"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="3075a-103">Aktualisieren von „deviceInstallState“</span><span class="sxs-lookup"><span data-stu-id="3075a-103">Update deviceInstallState</span></span>

> <span data-ttu-id="3075a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3075a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3075a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3075a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3075a-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="3075a-106">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3075a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3075a-107">Prerequisites</span></span>
<span data-ttu-id="3075a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3075a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3075a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3075a-110">Permission type</span></span>|<span data-ttu-id="3075a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3075a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3075a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3075a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3075a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3075a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3075a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3075a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3075a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3075a-115">Not supported.</span></span>|
|<span data-ttu-id="3075a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3075a-116">Application</span></span>|<span data-ttu-id="3075a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3075a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3075a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3075a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="3075a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3075a-119">Request headers</span></span>
|<span data-ttu-id="3075a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3075a-120">Header</span></span>|<span data-ttu-id="3075a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3075a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3075a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3075a-122">Authorization</span></span>|<span data-ttu-id="3075a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3075a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3075a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3075a-124">Accept</span></span>|<span data-ttu-id="3075a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3075a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3075a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3075a-126">Request body</span></span>
<span data-ttu-id="3075a-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) an.</span><span class="sxs-lookup"><span data-stu-id="3075a-127">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="3075a-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3075a-128">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="3075a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3075a-129">Property</span></span>|<span data-ttu-id="3075a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="3075a-130">Type</span></span>|<span data-ttu-id="3075a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3075a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3075a-132">id</span><span class="sxs-lookup"><span data-stu-id="3075a-132">id</span></span>|<span data-ttu-id="3075a-133">String</span><span class="sxs-lookup"><span data-stu-id="3075a-133">String</span></span>|<span data-ttu-id="3075a-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3075a-134">Key of the entity.</span></span>|
|<span data-ttu-id="3075a-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="3075a-135">deviceName</span></span>|<span data-ttu-id="3075a-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3075a-136">String</span></span>|<span data-ttu-id="3075a-137">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="3075a-137">Device name.</span></span>|
|<span data-ttu-id="3075a-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="3075a-138">deviceId</span></span>|<span data-ttu-id="3075a-139">String</span><span class="sxs-lookup"><span data-stu-id="3075a-139">String</span></span>|<span data-ttu-id="3075a-140">ID des Geräts</span><span class="sxs-lookup"><span data-stu-id="3075a-140">Device Id.</span></span>|
|<span data-ttu-id="3075a-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3075a-141">lastSyncDateTime</span></span>|<span data-ttu-id="3075a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3075a-142">DateTimeOffset</span></span>|<span data-ttu-id="3075a-143">Datum und Uhrzeit der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="3075a-143">Last sync date and time.</span></span>|
|<span data-ttu-id="3075a-144">installState</span><span class="sxs-lookup"><span data-stu-id="3075a-144">installState</span></span>|[<span data-ttu-id="3075a-145">installState</span><span class="sxs-lookup"><span data-stu-id="3075a-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="3075a-146">Installationsstatus des E-Books.</span><span class="sxs-lookup"><span data-stu-id="3075a-146">The install state of the eBook.</span></span> <span data-ttu-id="3075a-147">Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="3075a-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="3075a-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="3075a-148">errorCode</span></span>|<span data-ttu-id="3075a-149">String</span><span class="sxs-lookup"><span data-stu-id="3075a-149">String</span></span>|<span data-ttu-id="3075a-150">Fehlercode von Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="3075a-150">The error code for install failures.</span></span>|
|<span data-ttu-id="3075a-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="3075a-151">osVersion</span></span>|<span data-ttu-id="3075a-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3075a-152">String</span></span>|<span data-ttu-id="3075a-153">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="3075a-153">OS Version.</span></span>|
|<span data-ttu-id="3075a-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="3075a-154">osDescription</span></span>|<span data-ttu-id="3075a-155">String</span><span class="sxs-lookup"><span data-stu-id="3075a-155">String</span></span>|<span data-ttu-id="3075a-156">Beschreibung des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="3075a-156">OS Description.</span></span>|
|<span data-ttu-id="3075a-157">userName</span><span class="sxs-lookup"><span data-stu-id="3075a-157">userName</span></span>|<span data-ttu-id="3075a-158">String</span><span class="sxs-lookup"><span data-stu-id="3075a-158">String</span></span>|<span data-ttu-id="3075a-159">Name des Gerätebenutzers</span><span class="sxs-lookup"><span data-stu-id="3075a-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="3075a-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="3075a-160">Response</span></span>
<span data-ttu-id="3075a-161">Bei erfolgreicher Ausführung gibt die Methode den Antworttext `200 OK` und ein aktualisiertes Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3075a-161">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3075a-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3075a-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="3075a-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3075a-163">Request</span></span>
<span data-ttu-id="3075a-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3075a-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a><span data-ttu-id="3075a-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="3075a-165">Response</span></span>
<span data-ttu-id="3075a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3075a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```




