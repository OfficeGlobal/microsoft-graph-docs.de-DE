---
title: Erstellen von „deviceInstallState“
description: Diese Methode erstellt ein neues Objekt des Typs deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e7e37857cfa7d7c8820844f506b59d50933c5866
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962541"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="a8fe0-103">Erstellen von „deviceInstallState“</span><span class="sxs-lookup"><span data-stu-id="a8fe0-103">Create deviceInstallState</span></span>

> <span data-ttu-id="a8fe0-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a8fe0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8fe0-105">Diese Methode erstellt ein neues Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="a8fe0-105">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8fe0-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a8fe0-106">Prerequisites</span></span>
<span data-ttu-id="a8fe0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8fe0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8fe0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8fe0-109">Permission type</span></span>|<span data-ttu-id="a8fe0-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8fe0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8fe0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8fe0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a8fe0-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8fe0-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a8fe0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8fe0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8fe0-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8fe0-114">Not supported.</span></span>|
|<span data-ttu-id="a8fe0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8fe0-115">Application</span></span>|<span data-ttu-id="a8fe0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8fe0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8fe0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8fe0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="a8fe0-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8fe0-118">Request headers</span></span>
|<span data-ttu-id="a8fe0-119">Header</span><span class="sxs-lookup"><span data-stu-id="a8fe0-119">Header</span></span>|<span data-ttu-id="a8fe0-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a8fe0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8fe0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8fe0-121">Authorization</span></span>|<span data-ttu-id="a8fe0-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a8fe0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8fe0-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a8fe0-123">Accept</span></span>|<span data-ttu-id="a8fe0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a8fe0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8fe0-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8fe0-125">Request body</span></span>
<span data-ttu-id="a8fe0-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceInstallState“ an.</span><span class="sxs-lookup"><span data-stu-id="a8fe0-126">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="a8fe0-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceInstallState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="a8fe0-127">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="a8fe0-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8fe0-128">Property</span></span>|<span data-ttu-id="a8fe0-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a8fe0-129">Type</span></span>|<span data-ttu-id="a8fe0-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8fe0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8fe0-131">id</span><span class="sxs-lookup"><span data-stu-id="a8fe0-131">id</span></span>|<span data-ttu-id="a8fe0-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8fe0-132">String</span></span>|<span data-ttu-id="a8fe0-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a8fe0-133">Key of the entity.</span></span>|
|<span data-ttu-id="a8fe0-134">deviceName</span><span class="sxs-lookup"><span data-stu-id="a8fe0-134">deviceName</span></span>|<span data-ttu-id="a8fe0-135">String</span><span class="sxs-lookup"><span data-stu-id="a8fe0-135">String</span></span>|<span data-ttu-id="a8fe0-136">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="a8fe0-136">Device name.</span></span>|
|<span data-ttu-id="a8fe0-137">deviceId</span><span class="sxs-lookup"><span data-stu-id="a8fe0-137">deviceId</span></span>|<span data-ttu-id="a8fe0-138">String</span><span class="sxs-lookup"><span data-stu-id="a8fe0-138">String</span></span>|<span data-ttu-id="a8fe0-139">ID des Geräts</span><span class="sxs-lookup"><span data-stu-id="a8fe0-139">Device Id.</span></span>|
|<span data-ttu-id="a8fe0-140">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a8fe0-140">lastSyncDateTime</span></span>|<span data-ttu-id="a8fe0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8fe0-141">DateTimeOffset</span></span>|<span data-ttu-id="a8fe0-142">Datum und Uhrzeit der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="a8fe0-142">Last sync date and time.</span></span>|
|<span data-ttu-id="a8fe0-143">installState</span><span class="sxs-lookup"><span data-stu-id="a8fe0-143">installState</span></span>|[<span data-ttu-id="a8fe0-144">installState</span><span class="sxs-lookup"><span data-stu-id="a8fe0-144">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="a8fe0-145">Installationsstatus des E-Books.</span><span class="sxs-lookup"><span data-stu-id="a8fe0-145">The install state of the eBook.</span></span> <span data-ttu-id="a8fe0-146">Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a8fe0-146">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="a8fe0-147">errorCode</span><span class="sxs-lookup"><span data-stu-id="a8fe0-147">errorCode</span></span>|<span data-ttu-id="a8fe0-148">String</span><span class="sxs-lookup"><span data-stu-id="a8fe0-148">String</span></span>|<span data-ttu-id="a8fe0-149">Fehlercode von Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="a8fe0-149">The error code for install failures.</span></span>|
|<span data-ttu-id="a8fe0-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="a8fe0-150">osVersion</span></span>|<span data-ttu-id="a8fe0-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8fe0-151">String</span></span>|<span data-ttu-id="a8fe0-152">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="a8fe0-152">OS Version.</span></span>|
|<span data-ttu-id="a8fe0-153">osDescription</span><span class="sxs-lookup"><span data-stu-id="a8fe0-153">osDescription</span></span>|<span data-ttu-id="a8fe0-154">String</span><span class="sxs-lookup"><span data-stu-id="a8fe0-154">String</span></span>|<span data-ttu-id="a8fe0-155">Beschreibung des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="a8fe0-155">OS Description.</span></span>|
|<span data-ttu-id="a8fe0-156">userName</span><span class="sxs-lookup"><span data-stu-id="a8fe0-156">userName</span></span>|<span data-ttu-id="a8fe0-157">String</span><span class="sxs-lookup"><span data-stu-id="a8fe0-157">String</span></span>|<span data-ttu-id="a8fe0-158">Name des Gerätebenutzers</span><span class="sxs-lookup"><span data-stu-id="a8fe0-158">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="a8fe0-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8fe0-159">Response</span></span>
<span data-ttu-id="a8fe0-160">Bei erfolgreicher Ausführung gibt die Methode den Antworttext `201 Created` und ein Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a8fe0-160">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8fe0-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8fe0-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8fe0-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8fe0-162">Request</span></span>
<span data-ttu-id="a8fe0-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a8fe0-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a8fe0-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8fe0-164">Response</span></span>
<span data-ttu-id="a8fe0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8fe0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



