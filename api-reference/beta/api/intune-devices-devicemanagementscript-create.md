---
title: Erstellen von deviceManagementScript
description: Erstellen eines neuen DeviceManagementScript-Objekts.
author: tfitzmac
ms.openlocfilehash: 862b9c3ba50f879e92e47b50e6efaf0bcf41927a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315435"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="87bd2-103">Erstellen von deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="87bd2-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="87bd2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="87bd2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87bd2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87bd2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87bd2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="87bd2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87bd2-107">Erstellen eines neuen [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="87bd2-107">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87bd2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="87bd2-108">Prerequisites</span></span>
<span data-ttu-id="87bd2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87bd2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87bd2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87bd2-111">Permission type</span></span>|<span data-ttu-id="87bd2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87bd2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87bd2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87bd2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87bd2-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87bd2-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="87bd2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87bd2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87bd2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87bd2-116">Not supported.</span></span>|
|<span data-ttu-id="87bd2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87bd2-117">Application</span></span>|<span data-ttu-id="87bd2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="87bd2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87bd2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87bd2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="87bd2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87bd2-120">Request headers</span></span>
|<span data-ttu-id="87bd2-121">Header</span><span class="sxs-lookup"><span data-stu-id="87bd2-121">Header</span></span>|<span data-ttu-id="87bd2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="87bd2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87bd2-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="87bd2-123">Authorization</span></span>|<span data-ttu-id="87bd2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="87bd2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87bd2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87bd2-125">Accept</span></span>|<span data-ttu-id="87bd2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87bd2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87bd2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87bd2-127">Request body</span></span>
<span data-ttu-id="87bd2-128">Geben Sie im Textkörper Anforderung für das Objekt DeviceManagementScript eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="87bd2-128">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="87bd2-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DeviceManagementScript erstellen.</span><span class="sxs-lookup"><span data-stu-id="87bd2-129">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="87bd2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="87bd2-130">Property</span></span>|<span data-ttu-id="87bd2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="87bd2-131">Type</span></span>|<span data-ttu-id="87bd2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87bd2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87bd2-133">id</span><span class="sxs-lookup"><span data-stu-id="87bd2-133">id</span></span>|<span data-ttu-id="87bd2-134">String</span><span class="sxs-lookup"><span data-stu-id="87bd2-134">String</span></span>|<span data-ttu-id="87bd2-135">Eindeutiger Bezeichner für das Gerät Management-Skript.</span><span class="sxs-lookup"><span data-stu-id="87bd2-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="87bd2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="87bd2-136">displayName</span></span>|<span data-ttu-id="87bd2-137">String</span><span class="sxs-lookup"><span data-stu-id="87bd2-137">String</span></span>|<span data-ttu-id="87bd2-138">Name des Skripts Management Gerät.</span><span class="sxs-lookup"><span data-stu-id="87bd2-138">Name of the device management script.</span></span>|
|<span data-ttu-id="87bd2-139">description</span><span class="sxs-lookup"><span data-stu-id="87bd2-139">description</span></span>|<span data-ttu-id="87bd2-140">String</span><span class="sxs-lookup"><span data-stu-id="87bd2-140">String</span></span>|<span data-ttu-id="87bd2-141">Optionale Beschreibung für das Gerät Management-Skript.</span><span class="sxs-lookup"><span data-stu-id="87bd2-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="87bd2-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="87bd2-142">runSchedule</span></span>|[<span data-ttu-id="87bd2-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="87bd2-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="87bd2-144">Das Intervall für das Skript ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="87bd2-144">The interval for script to run.</span></span> <span data-ttu-id="87bd2-145">Wenn nicht definiert das Skript einmal ausgeführt wird</span><span class="sxs-lookup"><span data-stu-id="87bd2-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="87bd2-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="87bd2-146">scriptContent</span></span>|<span data-ttu-id="87bd2-147">Binär</span><span class="sxs-lookup"><span data-stu-id="87bd2-147">Binary</span></span>|<span data-ttu-id="87bd2-148">Der Skriptinhalt.</span><span class="sxs-lookup"><span data-stu-id="87bd2-148">The script content.</span></span>|
|<span data-ttu-id="87bd2-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87bd2-149">createdDateTime</span></span>|<span data-ttu-id="87bd2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87bd2-150">DateTimeOffset</span></span>|<span data-ttu-id="87bd2-151">Datum und Zeit für das Gerät Management-Skript erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="87bd2-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="87bd2-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87bd2-152">lastModifiedDateTime</span></span>|<span data-ttu-id="87bd2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87bd2-153">DateTimeOffset</span></span>|<span data-ttu-id="87bd2-154">Datum und Uhrzeit der letzten Änderung des Geräts Management-Skripts.</span><span class="sxs-lookup"><span data-stu-id="87bd2-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="87bd2-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="87bd2-155">runAsAccount</span></span>|[<span data-ttu-id="87bd2-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="87bd2-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="87bd2-157">Gibt den Typ des Ausführungskontexts, den das Gerät Management-Skript in ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="87bd2-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="87bd2-158">Mögliche Werte sind: `system` und `user`.</span><span class="sxs-lookup"><span data-stu-id="87bd2-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="87bd2-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="87bd2-159">enforceSignatureCheck</span></span>|<span data-ttu-id="87bd2-160">Boolesch</span><span class="sxs-lookup"><span data-stu-id="87bd2-160">Boolean</span></span>|<span data-ttu-id="87bd2-161">Geben Sie an, ob die Signatur Skript muss aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="87bd2-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="87bd2-162">fileName</span><span class="sxs-lookup"><span data-stu-id="87bd2-162">fileName</span></span>|<span data-ttu-id="87bd2-163">String</span><span class="sxs-lookup"><span data-stu-id="87bd2-163">String</span></span>|<span data-ttu-id="87bd2-164">Dateiname des Skripts.</span><span class="sxs-lookup"><span data-stu-id="87bd2-164">Script file name.</span></span>|



## <a name="response"></a><span data-ttu-id="87bd2-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="87bd2-165">Response</span></span>
<span data-ttu-id="87bd2-166">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="87bd2-166">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87bd2-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="87bd2-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="87bd2-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87bd2-168">Request</span></span>
<span data-ttu-id="87bd2-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87bd2-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 422

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value"
}
```

### <a name="response"></a><span data-ttu-id="87bd2-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="87bd2-170">Response</span></span>
<span data-ttu-id="87bd2-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="87bd2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 530

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value"
}
```





