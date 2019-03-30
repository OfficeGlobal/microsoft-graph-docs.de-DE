---
title: Erstellen von „deviceInstallState“
description: Diese Methode erstellt ein neues Objekt des Typs deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa2402605f77d9d901c4941ded593e8c1d787040
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986908"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="0e8ba-103">Erstellen von „deviceInstallState“</span><span class="sxs-lookup"><span data-stu-id="0e8ba-103">Create deviceInstallState</span></span>

> <span data-ttu-id="0e8ba-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0e8ba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e8ba-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0e8ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e8ba-106">Diese Methode erstellt ein neues Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="0e8ba-106">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e8ba-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0e8ba-107">Prerequisites</span></span>
<span data-ttu-id="0e8ba-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e8ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e8ba-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e8ba-110">Permission type</span></span>|<span data-ttu-id="0e8ba-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e8ba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e8ba-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e8ba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0e8ba-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e8ba-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0e8ba-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e8ba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e8ba-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e8ba-115">Not supported.</span></span>|
|<span data-ttu-id="0e8ba-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e8ba-116">Application</span></span>|<span data-ttu-id="0e8ba-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e8ba-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e8ba-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e8ba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="0e8ba-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e8ba-119">Request headers</span></span>
|<span data-ttu-id="0e8ba-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0e8ba-120">Header</span></span>|<span data-ttu-id="0e8ba-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0e8ba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e8ba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e8ba-122">Authorization</span></span>|<span data-ttu-id="0e8ba-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0e8ba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e8ba-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0e8ba-124">Accept</span></span>|<span data-ttu-id="0e8ba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0e8ba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e8ba-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e8ba-126">Request body</span></span>
<span data-ttu-id="0e8ba-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceInstallState“ an.</span><span class="sxs-lookup"><span data-stu-id="0e8ba-127">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="0e8ba-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceInstallState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="0e8ba-128">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="0e8ba-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e8ba-129">Property</span></span>|<span data-ttu-id="0e8ba-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0e8ba-130">Type</span></span>|<span data-ttu-id="0e8ba-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e8ba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e8ba-132">id</span><span class="sxs-lookup"><span data-stu-id="0e8ba-132">id</span></span>|<span data-ttu-id="0e8ba-133">String</span><span class="sxs-lookup"><span data-stu-id="0e8ba-133">String</span></span>|<span data-ttu-id="0e8ba-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0e8ba-134">Key of the entity.</span></span>|
|<span data-ttu-id="0e8ba-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="0e8ba-135">deviceName</span></span>|<span data-ttu-id="0e8ba-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e8ba-136">String</span></span>|<span data-ttu-id="0e8ba-137">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="0e8ba-137">Device name.</span></span>|
|<span data-ttu-id="0e8ba-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="0e8ba-138">deviceId</span></span>|<span data-ttu-id="0e8ba-139">String</span><span class="sxs-lookup"><span data-stu-id="0e8ba-139">String</span></span>|<span data-ttu-id="0e8ba-140">ID des Geräts</span><span class="sxs-lookup"><span data-stu-id="0e8ba-140">Device Id.</span></span>|
|<span data-ttu-id="0e8ba-141">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0e8ba-141">lastSyncDateTime</span></span>|<span data-ttu-id="0e8ba-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e8ba-142">DateTimeOffset</span></span>|<span data-ttu-id="0e8ba-143">Datum und Uhrzeit der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="0e8ba-143">Last sync date and time.</span></span>|
|<span data-ttu-id="0e8ba-144">installState</span><span class="sxs-lookup"><span data-stu-id="0e8ba-144">installState</span></span>|[<span data-ttu-id="0e8ba-145">installState</span><span class="sxs-lookup"><span data-stu-id="0e8ba-145">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="0e8ba-146">Installationsstatus des E-Books.</span><span class="sxs-lookup"><span data-stu-id="0e8ba-146">The install state of the eBook.</span></span> <span data-ttu-id="0e8ba-147">Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0e8ba-147">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="0e8ba-148">errorCode</span><span class="sxs-lookup"><span data-stu-id="0e8ba-148">errorCode</span></span>|<span data-ttu-id="0e8ba-149">String</span><span class="sxs-lookup"><span data-stu-id="0e8ba-149">String</span></span>|<span data-ttu-id="0e8ba-150">Fehlercode von Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="0e8ba-150">The error code for install failures.</span></span>|
|<span data-ttu-id="0e8ba-151">osVersion</span><span class="sxs-lookup"><span data-stu-id="0e8ba-151">osVersion</span></span>|<span data-ttu-id="0e8ba-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e8ba-152">String</span></span>|<span data-ttu-id="0e8ba-153">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="0e8ba-153">OS Version.</span></span>|
|<span data-ttu-id="0e8ba-154">osDescription</span><span class="sxs-lookup"><span data-stu-id="0e8ba-154">osDescription</span></span>|<span data-ttu-id="0e8ba-155">String</span><span class="sxs-lookup"><span data-stu-id="0e8ba-155">String</span></span>|<span data-ttu-id="0e8ba-156">Beschreibung des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="0e8ba-156">OS Description.</span></span>|
|<span data-ttu-id="0e8ba-157">userName</span><span class="sxs-lookup"><span data-stu-id="0e8ba-157">userName</span></span>|<span data-ttu-id="0e8ba-158">String</span><span class="sxs-lookup"><span data-stu-id="0e8ba-158">String</span></span>|<span data-ttu-id="0e8ba-159">Name des Gerätebenutzers</span><span class="sxs-lookup"><span data-stu-id="0e8ba-159">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="0e8ba-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e8ba-160">Response</span></span>
<span data-ttu-id="0e8ba-161">Bei erfolgreicher Ausführung gibt die Methode den Antworttext `201 Created` und ein Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0e8ba-161">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e8ba-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e8ba-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e8ba-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e8ba-163">Request</span></span>
<span data-ttu-id="0e8ba-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e8ba-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="0e8ba-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e8ba-165">Response</span></span>
<span data-ttu-id="0e8ba-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e8ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




