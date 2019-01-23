---
title: Aktualisieren von „deviceInstallState“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceInstallState.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d73f1cc881d918f385bfdc8d98cf9a1451a554e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394789"
---
# <a name="update-deviceinstallstate"></a><span data-ttu-id="37c21-103">Aktualisieren von „deviceInstallState“</span><span class="sxs-lookup"><span data-stu-id="37c21-103">Update deviceInstallState</span></span>

> <span data-ttu-id="37c21-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="37c21-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37c21-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="37c21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37c21-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="37c21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37c21-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="37c21-107">Update the properties of a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37c21-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="37c21-108">Prerequisites</span></span>
<span data-ttu-id="37c21-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="37c21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="37c21-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="37c21-111">Permission type</span></span>|<span data-ttu-id="37c21-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="37c21-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37c21-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="37c21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37c21-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c21-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="37c21-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="37c21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37c21-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37c21-116">Not supported.</span></span>|
|<span data-ttu-id="37c21-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="37c21-117">Application</span></span>|<span data-ttu-id="37c21-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="37c21-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37c21-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="37c21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="37c21-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="37c21-120">Request headers</span></span>
|<span data-ttu-id="37c21-121">Header</span><span class="sxs-lookup"><span data-stu-id="37c21-121">Header</span></span>|<span data-ttu-id="37c21-122">Wert</span><span class="sxs-lookup"><span data-stu-id="37c21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37c21-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="37c21-123">Authorization</span></span>|<span data-ttu-id="37c21-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="37c21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37c21-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="37c21-125">Accept</span></span>|<span data-ttu-id="37c21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37c21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37c21-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="37c21-127">Request body</span></span>
<span data-ttu-id="37c21-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) an.</span><span class="sxs-lookup"><span data-stu-id="37c21-128">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

<span data-ttu-id="37c21-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="37c21-129">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span></span>

|<span data-ttu-id="37c21-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="37c21-130">Property</span></span>|<span data-ttu-id="37c21-131">Typ</span><span class="sxs-lookup"><span data-stu-id="37c21-131">Type</span></span>|<span data-ttu-id="37c21-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="37c21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37c21-133">id</span><span class="sxs-lookup"><span data-stu-id="37c21-133">id</span></span>|<span data-ttu-id="37c21-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37c21-134">String</span></span>|<span data-ttu-id="37c21-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="37c21-135">Key of the entity.</span></span>|
|<span data-ttu-id="37c21-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="37c21-136">deviceName</span></span>|<span data-ttu-id="37c21-137">String</span><span class="sxs-lookup"><span data-stu-id="37c21-137">String</span></span>|<span data-ttu-id="37c21-138">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="37c21-138">Device name.</span></span>|
|<span data-ttu-id="37c21-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="37c21-139">deviceId</span></span>|<span data-ttu-id="37c21-140">String</span><span class="sxs-lookup"><span data-stu-id="37c21-140">String</span></span>|<span data-ttu-id="37c21-141">ID des Geräts</span><span class="sxs-lookup"><span data-stu-id="37c21-141">Device Id.</span></span>|
|<span data-ttu-id="37c21-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="37c21-142">lastSyncDateTime</span></span>|<span data-ttu-id="37c21-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37c21-143">DateTimeOffset</span></span>|<span data-ttu-id="37c21-144">Datum und Uhrzeit der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="37c21-144">Last sync date and time.</span></span>|
|<span data-ttu-id="37c21-145">installState</span><span class="sxs-lookup"><span data-stu-id="37c21-145">installState</span></span>|[<span data-ttu-id="37c21-146">installState</span><span class="sxs-lookup"><span data-stu-id="37c21-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="37c21-147">Installationsstatus des E-Books.</span><span class="sxs-lookup"><span data-stu-id="37c21-147">The install state of the eBook.</span></span> <span data-ttu-id="37c21-148">Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="37c21-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="37c21-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="37c21-149">errorCode</span></span>|<span data-ttu-id="37c21-150">String</span><span class="sxs-lookup"><span data-stu-id="37c21-150">String</span></span>|<span data-ttu-id="37c21-151">Fehlercode von Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="37c21-151">The error code for install failures.</span></span>|
|<span data-ttu-id="37c21-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="37c21-152">osVersion</span></span>|<span data-ttu-id="37c21-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="37c21-153">String</span></span>|<span data-ttu-id="37c21-154">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="37c21-154">OS Version.</span></span>|
|<span data-ttu-id="37c21-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="37c21-155">osDescription</span></span>|<span data-ttu-id="37c21-156">String</span><span class="sxs-lookup"><span data-stu-id="37c21-156">String</span></span>|<span data-ttu-id="37c21-157">Beschreibung des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="37c21-157">OS Description.</span></span>|
|<span data-ttu-id="37c21-158">userName</span><span class="sxs-lookup"><span data-stu-id="37c21-158">userName</span></span>|<span data-ttu-id="37c21-159">String</span><span class="sxs-lookup"><span data-stu-id="37c21-159">String</span></span>|<span data-ttu-id="37c21-160">Name des Gerätebenutzers</span><span class="sxs-lookup"><span data-stu-id="37c21-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="37c21-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="37c21-161">Response</span></span>
<span data-ttu-id="37c21-162">Bei erfolgreicher Ausführung gibt die Methode den Antworttext `200 OK` und ein aktualisiertes Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="37c21-162">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37c21-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="37c21-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="37c21-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="37c21-164">Request</span></span>
<span data-ttu-id="37c21-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="37c21-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37c21-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="37c21-166">Response</span></span>
<span data-ttu-id="37c21-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="37c21-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




