---
title: Erstellen von „deviceInstallState“
description: Diese Methode erstellt ein neues Objekt des Typs deviceInstallState.
ms.openlocfilehash: b210ca932ee6132bd4b5c09988fae3c0bae9ca25
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063412"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="0b421-103">Erstellen von „deviceInstallState“</span><span class="sxs-lookup"><span data-stu-id="0b421-103">Create deviceInstallState</span></span>

> <span data-ttu-id="0b421-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0b421-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b421-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0b421-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b421-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="0b421-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b421-107">Diese Methode erstellt ein neues Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="0b421-107">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b421-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0b421-108">Prerequisites</span></span>
<span data-ttu-id="0b421-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b421-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b421-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0b421-111">Permission type</span></span>|<span data-ttu-id="0b421-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0b421-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b421-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0b421-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b421-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b421-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0b421-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0b421-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b421-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b421-116">Not supported.</span></span>|
|<span data-ttu-id="0b421-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0b421-117">Application</span></span>|<span data-ttu-id="0b421-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0b421-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b421-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b421-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="0b421-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0b421-120">Request headers</span></span>
|<span data-ttu-id="0b421-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0b421-121">Header</span></span>|<span data-ttu-id="0b421-122">Wert</span><span class="sxs-lookup"><span data-stu-id="0b421-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b421-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b421-123">Authorization</span></span>|<span data-ttu-id="0b421-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0b421-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b421-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b421-125">Accept</span></span>|<span data-ttu-id="0b421-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b421-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b421-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0b421-127">Request body</span></span>
<span data-ttu-id="0b421-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceInstallState“ an.</span><span class="sxs-lookup"><span data-stu-id="0b421-128">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="0b421-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceInstallState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="0b421-129">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="0b421-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0b421-130">Property</span></span>|<span data-ttu-id="0b421-131">Typ</span><span class="sxs-lookup"><span data-stu-id="0b421-131">Type</span></span>|<span data-ttu-id="0b421-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0b421-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b421-133">id</span><span class="sxs-lookup"><span data-stu-id="0b421-133">id</span></span>|<span data-ttu-id="0b421-134">String</span><span class="sxs-lookup"><span data-stu-id="0b421-134">String</span></span>|<span data-ttu-id="0b421-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0b421-135">Key of the entity.</span></span>|
|<span data-ttu-id="0b421-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="0b421-136">deviceName</span></span>|<span data-ttu-id="0b421-137">String</span><span class="sxs-lookup"><span data-stu-id="0b421-137">String</span></span>|<span data-ttu-id="0b421-138">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="0b421-138">Device name.</span></span>|
|<span data-ttu-id="0b421-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="0b421-139">deviceId</span></span>|<span data-ttu-id="0b421-140">String</span><span class="sxs-lookup"><span data-stu-id="0b421-140">String</span></span>|<span data-ttu-id="0b421-141">ID des Geräts</span><span class="sxs-lookup"><span data-stu-id="0b421-141">Device Id.</span></span>|
|<span data-ttu-id="0b421-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="0b421-142">lastSyncDateTime</span></span>|<span data-ttu-id="0b421-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b421-143">DateTimeOffset</span></span>|<span data-ttu-id="0b421-144">Datum und Uhrzeit der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="0b421-144">Last sync date and time.</span></span>|
|<span data-ttu-id="0b421-145">installState</span><span class="sxs-lookup"><span data-stu-id="0b421-145">installState</span></span>|[<span data-ttu-id="0b421-146">installState</span><span class="sxs-lookup"><span data-stu-id="0b421-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="0b421-147">Installationsstatus des E-Books.</span><span class="sxs-lookup"><span data-stu-id="0b421-147">The install state of the eBook.</span></span> <span data-ttu-id="0b421-148">Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0b421-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="0b421-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="0b421-149">errorCode</span></span>|<span data-ttu-id="0b421-150">String</span><span class="sxs-lookup"><span data-stu-id="0b421-150">String</span></span>|<span data-ttu-id="0b421-151">Fehlercode von Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="0b421-151">The error code for install failures.</span></span>|
|<span data-ttu-id="0b421-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="0b421-152">osVersion</span></span>|<span data-ttu-id="0b421-153">String</span><span class="sxs-lookup"><span data-stu-id="0b421-153">String</span></span>|<span data-ttu-id="0b421-154">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="0b421-154">OS Version.</span></span>|
|<span data-ttu-id="0b421-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="0b421-155">osDescription</span></span>|<span data-ttu-id="0b421-156">String</span><span class="sxs-lookup"><span data-stu-id="0b421-156">String</span></span>|<span data-ttu-id="0b421-157">Beschreibung des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="0b421-157">OS Description.</span></span>|
|<span data-ttu-id="0b421-158">userName</span><span class="sxs-lookup"><span data-stu-id="0b421-158">userName</span></span>|<span data-ttu-id="0b421-159">String</span><span class="sxs-lookup"><span data-stu-id="0b421-159">String</span></span>|<span data-ttu-id="0b421-160">Name des Gerätebenutzers</span><span class="sxs-lookup"><span data-stu-id="0b421-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="0b421-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b421-161">Response</span></span>
<span data-ttu-id="0b421-162">Bei erfolgreicher Ausführung gibt die Methode den Antworttext `201 Created` und ein Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0b421-162">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b421-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0b421-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b421-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0b421-164">Request</span></span>
<span data-ttu-id="0b421-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0b421-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b421-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="0b421-166">Response</span></span>
<span data-ttu-id="0b421-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0b421-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





