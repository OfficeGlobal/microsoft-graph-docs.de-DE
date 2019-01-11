---
title: Erstellen von „deviceInstallState“
description: Diese Methode erstellt ein neues Objekt des Typs deviceInstallState.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 244a03aa7c1f42c6e71591a3358ab7fca67a9b48
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853886"
---
# <a name="create-deviceinstallstate"></a><span data-ttu-id="096f4-103">Erstellen von „deviceInstallState“</span><span class="sxs-lookup"><span data-stu-id="096f4-103">Create deviceInstallState</span></span>

> <span data-ttu-id="096f4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="096f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="096f4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="096f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="096f4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="096f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="096f4-107">Diese Methode erstellt ein neues Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md).</span><span class="sxs-lookup"><span data-stu-id="096f4-107">Create a new [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="096f4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="096f4-108">Prerequisites</span></span>
<span data-ttu-id="096f4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="096f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="096f4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="096f4-111">Permission type</span></span>|<span data-ttu-id="096f4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="096f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="096f4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="096f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="096f4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="096f4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="096f4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="096f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="096f4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="096f4-116">Not supported.</span></span>|
|<span data-ttu-id="096f4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="096f4-117">Application</span></span>|<span data-ttu-id="096f4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="096f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="096f4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="096f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="096f4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="096f4-120">Request headers</span></span>
|<span data-ttu-id="096f4-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="096f4-121">Header</span></span>|<span data-ttu-id="096f4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="096f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="096f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="096f4-123">Authorization</span></span>|<span data-ttu-id="096f4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="096f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="096f4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="096f4-125">Accept</span></span>|<span data-ttu-id="096f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="096f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="096f4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="096f4-127">Request body</span></span>
<span data-ttu-id="096f4-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceInstallState“ an.</span><span class="sxs-lookup"><span data-stu-id="096f4-128">In the request body, supply a JSON representation for the deviceInstallState object.</span></span>

<span data-ttu-id="096f4-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceInstallState“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="096f4-129">The following table shows the properties that are required when you create the deviceInstallState.</span></span>

|<span data-ttu-id="096f4-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="096f4-130">Property</span></span>|<span data-ttu-id="096f4-131">Typ</span><span class="sxs-lookup"><span data-stu-id="096f4-131">Type</span></span>|<span data-ttu-id="096f4-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="096f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="096f4-133">id</span><span class="sxs-lookup"><span data-stu-id="096f4-133">id</span></span>|<span data-ttu-id="096f4-134">String</span><span class="sxs-lookup"><span data-stu-id="096f4-134">String</span></span>|<span data-ttu-id="096f4-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="096f4-135">Key of the entity.</span></span>|
|<span data-ttu-id="096f4-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="096f4-136">deviceName</span></span>|<span data-ttu-id="096f4-137">String</span><span class="sxs-lookup"><span data-stu-id="096f4-137">String</span></span>|<span data-ttu-id="096f4-138">Name des Geräts</span><span class="sxs-lookup"><span data-stu-id="096f4-138">Device name.</span></span>|
|<span data-ttu-id="096f4-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="096f4-139">deviceId</span></span>|<span data-ttu-id="096f4-140">String</span><span class="sxs-lookup"><span data-stu-id="096f4-140">String</span></span>|<span data-ttu-id="096f4-141">ID des Geräts</span><span class="sxs-lookup"><span data-stu-id="096f4-141">Device Id.</span></span>|
|<span data-ttu-id="096f4-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="096f4-142">lastSyncDateTime</span></span>|<span data-ttu-id="096f4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="096f4-143">DateTimeOffset</span></span>|<span data-ttu-id="096f4-144">Datum und Uhrzeit der letzten Synchronisierung</span><span class="sxs-lookup"><span data-stu-id="096f4-144">Last sync date and time.</span></span>|
|<span data-ttu-id="096f4-145">installState</span><span class="sxs-lookup"><span data-stu-id="096f4-145">installState</span></span>|[<span data-ttu-id="096f4-146">installState</span><span class="sxs-lookup"><span data-stu-id="096f4-146">installState</span></span>](../resources/intune-books-installstate.md)|<span data-ttu-id="096f4-147">Installationsstatus des E-Books.</span><span class="sxs-lookup"><span data-stu-id="096f4-147">The install state of the eBook.</span></span> <span data-ttu-id="096f4-148">Mögliche Werte sind: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed` und `unknown`.</span><span class="sxs-lookup"><span data-stu-id="096f4-148">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="096f4-149">errorCode</span><span class="sxs-lookup"><span data-stu-id="096f4-149">errorCode</span></span>|<span data-ttu-id="096f4-150">String</span><span class="sxs-lookup"><span data-stu-id="096f4-150">String</span></span>|<span data-ttu-id="096f4-151">Fehlercode von Installationsfehlern</span><span class="sxs-lookup"><span data-stu-id="096f4-151">The error code for install failures.</span></span>|
|<span data-ttu-id="096f4-152">osVersion</span><span class="sxs-lookup"><span data-stu-id="096f4-152">osVersion</span></span>|<span data-ttu-id="096f4-153">String</span><span class="sxs-lookup"><span data-stu-id="096f4-153">String</span></span>|<span data-ttu-id="096f4-154">Betriebssystemversion</span><span class="sxs-lookup"><span data-stu-id="096f4-154">OS Version.</span></span>|
|<span data-ttu-id="096f4-155">osDescription</span><span class="sxs-lookup"><span data-stu-id="096f4-155">osDescription</span></span>|<span data-ttu-id="096f4-156">String</span><span class="sxs-lookup"><span data-stu-id="096f4-156">String</span></span>|<span data-ttu-id="096f4-157">Beschreibung des Betriebssystems</span><span class="sxs-lookup"><span data-stu-id="096f4-157">OS Description.</span></span>|
|<span data-ttu-id="096f4-158">userName</span><span class="sxs-lookup"><span data-stu-id="096f4-158">userName</span></span>|<span data-ttu-id="096f4-159">String</span><span class="sxs-lookup"><span data-stu-id="096f4-159">String</span></span>|<span data-ttu-id="096f4-160">Name des Gerätebenutzers</span><span class="sxs-lookup"><span data-stu-id="096f4-160">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="096f4-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="096f4-161">Response</span></span>
<span data-ttu-id="096f4-162">Bei erfolgreicher Ausführung gibt die Methode den Antworttext `201 Created` und ein Objekt des Typs [deviceInstallState](../resources/intune-books-deviceinstallstate.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="096f4-162">If successful, this method returns a `201 Created` response code and a [deviceInstallState](../resources/intune-books-deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="096f4-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="096f4-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="096f4-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="096f4-164">Request</span></span>
<span data-ttu-id="096f4-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="096f4-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="096f4-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="096f4-166">Response</span></span>
<span data-ttu-id="096f4-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="096f4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





