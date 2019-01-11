---
title: Erstellen von „deviceInstallState“
description: Diese Methode erstellt ein neues Objekt des Typs deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 49979b883ffef895124d8bb57837d5c5103a0d67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825480"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="eaa34-103">Erstellen von „deviceInstallState“</span><span class="sxs-lookup"><span data-stu-id="eaa34-103">Create deviceInstallState</span></span>

> <span data-ttu-id="eaa34-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eaa34-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eaa34-105">Diese Methode erstellt ein neues Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="eaa34-105">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eaa34-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eaa34-106">Prerequisites</span></span>
<span data-ttu-id="eaa34-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaa34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaa34-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eaa34-109">Permission type</span></span>|<span data-ttu-id="eaa34-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eaa34-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eaa34-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eaa34-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eaa34-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaa34-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eaa34-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eaa34-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eaa34-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eaa34-114">Not supported.</span></span>|
|<span data-ttu-id="eaa34-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eaa34-115">Application</span></span>|<span data-ttu-id="eaa34-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eaa34-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eaa34-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eaa34-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="eaa34-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eaa34-118">Request headers</span></span>
|<span data-ttu-id="eaa34-119">Header</span><span class="sxs-lookup"><span data-stu-id="eaa34-119">Header</span></span>|<span data-ttu-id="eaa34-120">Wert</span><span class="sxs-lookup"><span data-stu-id="eaa34-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eaa34-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaa34-121">Authorization</span></span>|<span data-ttu-id="eaa34-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eaa34-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eaa34-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eaa34-123">Accept</span></span>|<span data-ttu-id="eaa34-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eaa34-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eaa34-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eaa34-125">Request body</span></span>
<span data-ttu-id="eaa34-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceInstallState“ an.</span><span class="sxs-lookup"><span data-stu-id="eaa34-126">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="eaa34-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceInstallState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="eaa34-127">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="eaa34-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eaa34-128">Property</span></span>|<span data-ttu-id="eaa34-129">Typ</span><span class="sxs-lookup"><span data-stu-id="eaa34-129">Type</span></span>|<span data-ttu-id="eaa34-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eaa34-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaa34-131">id</span><span class="sxs-lookup"><span data-stu-id="eaa34-131">id</span></span>|<span data-ttu-id="eaa34-132">String</span><span class="sxs-lookup"><span data-stu-id="eaa34-132">String</span></span>|<span data-ttu-id="eaa34-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="eaa34-133">Key of the entity.</span></span>|
|<span data-ttu-id="eaa34-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="eaa34-134">deviceName</span></span>|<span data-ttu-id="eaa34-135">String</span><span class="sxs-lookup"><span data-stu-id="eaa34-135">String</span></span>|<span data-ttu-id="eaa34-136">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="eaa34-136">Device name.</span></span>|
|<span data-ttu-id="eaa34-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="eaa34-137">deviceId</span></span>|<span data-ttu-id="eaa34-138">String</span><span class="sxs-lookup"><span data-stu-id="eaa34-138">String</span></span>|<span data-ttu-id="eaa34-139">ID des Geräts</span><span class="sxs-lookup"><span data-stu-id="eaa34-139">Device Id.</span></span>|
|<span data-ttu-id="eaa34-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="eaa34-140">lastSyncDateTime</span></span>|<span data-ttu-id="eaa34-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eaa34-141">DateTimeOffset</span></span>|<span data-ttu-id="eaa34-142">Datum und Uhrzeit der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="eaa34-142">Last sync date and time.</span></span>|
|<span data-ttu-id="eaa34-143">installState</span><span class="sxs-lookup"><span data-stu-id="eaa34-143">installState</span></span>|[<span data-ttu-id="eaa34-144">installState</span><span class="sxs-lookup"><span data-stu-id="eaa34-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="eaa34-145">Installationsstatus des E-Books.</span><span class="sxs-lookup"><span data-stu-id="eaa34-145">The install state of the eBook.</span></span> <span data-ttu-id="eaa34-146">Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="eaa34-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="eaa34-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="eaa34-147">errorCode</span></span>|<span data-ttu-id="eaa34-148">String</span><span class="sxs-lookup"><span data-stu-id="eaa34-148">String</span></span>|<span data-ttu-id="eaa34-149">Fehlercode von Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="eaa34-149">The error code for install failures.</span></span>|
|<span data-ttu-id="eaa34-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="eaa34-150">osVersion</span></span>|<span data-ttu-id="eaa34-151">String</span><span class="sxs-lookup"><span data-stu-id="eaa34-151">String</span></span>|<span data-ttu-id="eaa34-152">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="eaa34-152">OS Version.</span></span>|
|<span data-ttu-id="eaa34-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="eaa34-153">osDescription</span></span>|<span data-ttu-id="eaa34-154">String</span><span class="sxs-lookup"><span data-stu-id="eaa34-154">String</span></span>|<span data-ttu-id="eaa34-155">Beschreibung des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="eaa34-155">OS Description.</span></span>|
|<span data-ttu-id="eaa34-156">userName</span><span class="sxs-lookup"><span data-stu-id="eaa34-156">userName</span></span>|<span data-ttu-id="eaa34-157">String</span><span class="sxs-lookup"><span data-stu-id="eaa34-157">String</span></span>|<span data-ttu-id="eaa34-158">Name des Gerätebenutzers</span><span class="sxs-lookup"><span data-stu-id="eaa34-158">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="eaa34-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="eaa34-159">Response</span></span>
<span data-ttu-id="eaa34-160">Bei erfolgreicher Ausführung gibt die Methode den Antworttext `201 Created` und ein Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eaa34-160">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaa34-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eaa34-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="eaa34-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eaa34-162">Request</span></span>
<span data-ttu-id="eaa34-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eaa34-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
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

### <a name="response"></a><span data-ttu-id="eaa34-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="eaa34-164">Response</span></span>
<span data-ttu-id="eaa34-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eaa34-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



