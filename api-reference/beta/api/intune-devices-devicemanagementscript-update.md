---
title: DeviceManagementScript aktualisieren
description: Aktualisieren Sie die Eigenschaften eines DeviceManagementScript-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fa19b1d34ebd3b00a4c2d03f32730647dec45bda
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924223"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="9cde6-103">DeviceManagementScript aktualisieren</span><span class="sxs-lookup"><span data-stu-id="9cde6-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="9cde6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9cde6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9cde6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9cde6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9cde6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9cde6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9cde6-107">Aktualisieren Sie die Eigenschaften eines [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="9cde6-107">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9cde6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9cde6-108">Prerequisites</span></span>
<span data-ttu-id="9cde6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9cde6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cde6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9cde6-111">Permission type</span></span>|<span data-ttu-id="9cde6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9cde6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cde6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9cde6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cde6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cde6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9cde6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9cde6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cde6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9cde6-116">Not supported.</span></span>|
|<span data-ttu-id="9cde6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9cde6-117">Application</span></span>|<span data-ttu-id="9cde6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9cde6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cde6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9cde6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="9cde6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9cde6-120">Request headers</span></span>
|<span data-ttu-id="9cde6-121">Header</span><span class="sxs-lookup"><span data-stu-id="9cde6-121">Header</span></span>|<span data-ttu-id="9cde6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9cde6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cde6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cde6-123">Authorization</span></span>|<span data-ttu-id="9cde6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9cde6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cde6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9cde6-125">Accept</span></span>|<span data-ttu-id="9cde6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cde6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cde6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9cde6-127">Request body</span></span>
<span data-ttu-id="9cde6-128">Geben Sie im Textkörper Anforderung für das Objekt [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="9cde6-128">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="9cde6-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="9cde6-129">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="9cde6-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9cde6-130">Property</span></span>|<span data-ttu-id="9cde6-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9cde6-131">Type</span></span>|<span data-ttu-id="9cde6-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9cde6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cde6-133">id</span><span class="sxs-lookup"><span data-stu-id="9cde6-133">id</span></span>|<span data-ttu-id="9cde6-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9cde6-134">String</span></span>|<span data-ttu-id="9cde6-135">Eindeutiger Bezeichner für das Gerät Management-Skript.</span><span class="sxs-lookup"><span data-stu-id="9cde6-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="9cde6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="9cde6-136">displayName</span></span>|<span data-ttu-id="9cde6-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9cde6-137">String</span></span>|<span data-ttu-id="9cde6-138">Name des Skripts Management Gerät.</span><span class="sxs-lookup"><span data-stu-id="9cde6-138">Name of the device management script.</span></span>|
|<span data-ttu-id="9cde6-139">description</span><span class="sxs-lookup"><span data-stu-id="9cde6-139">description</span></span>|<span data-ttu-id="9cde6-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9cde6-140">String</span></span>|<span data-ttu-id="9cde6-141">Optionale Beschreibung für das Gerät Management-Skript.</span><span class="sxs-lookup"><span data-stu-id="9cde6-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="9cde6-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="9cde6-142">runSchedule</span></span>|[<span data-ttu-id="9cde6-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="9cde6-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="9cde6-144">Das Intervall für das Skript ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="9cde6-144">The interval for script to run.</span></span> <span data-ttu-id="9cde6-145">Wenn nicht definiert das Skript einmal ausgeführt wird</span><span class="sxs-lookup"><span data-stu-id="9cde6-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="9cde6-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="9cde6-146">scriptContent</span></span>|<span data-ttu-id="9cde6-147">Binär</span><span class="sxs-lookup"><span data-stu-id="9cde6-147">Binary</span></span>|<span data-ttu-id="9cde6-148">Der Skriptinhalt.</span><span class="sxs-lookup"><span data-stu-id="9cde6-148">The script content.</span></span>|
|<span data-ttu-id="9cde6-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9cde6-149">createdDateTime</span></span>|<span data-ttu-id="9cde6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cde6-150">DateTimeOffset</span></span>|<span data-ttu-id="9cde6-151">Datum und Zeit für das Gerät Management-Skript erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="9cde6-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="9cde6-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9cde6-152">lastModifiedDateTime</span></span>|<span data-ttu-id="9cde6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cde6-153">DateTimeOffset</span></span>|<span data-ttu-id="9cde6-154">Datum und Uhrzeit der letzten Änderung des Geräts Management-Skripts.</span><span class="sxs-lookup"><span data-stu-id="9cde6-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="9cde6-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="9cde6-155">runAsAccount</span></span>|[<span data-ttu-id="9cde6-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="9cde6-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="9cde6-157">Gibt den Typ des Ausführungskontexts, den das Gerät Management-Skript in ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="9cde6-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="9cde6-158">Mögliche Werte sind: `system` und `user`.</span><span class="sxs-lookup"><span data-stu-id="9cde6-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="9cde6-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="9cde6-159">enforceSignatureCheck</span></span>|<span data-ttu-id="9cde6-160">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="9cde6-160">Boolean</span></span>|<span data-ttu-id="9cde6-161">Geben Sie an, ob die Signatur Skript muss aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="9cde6-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="9cde6-162">fileName</span><span class="sxs-lookup"><span data-stu-id="9cde6-162">fileName</span></span>|<span data-ttu-id="9cde6-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="9cde6-163">String</span></span>|<span data-ttu-id="9cde6-164">Dateiname des Skripts.</span><span class="sxs-lookup"><span data-stu-id="9cde6-164">Script file name.</span></span>|



## <a name="response"></a><span data-ttu-id="9cde6-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cde6-165">Response</span></span>
<span data-ttu-id="9cde6-166">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="9cde6-166">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cde6-167">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9cde6-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="9cde6-168">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9cde6-168">Request</span></span>
<span data-ttu-id="9cde6-169">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9cde6-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 361

{
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

### <a name="response"></a><span data-ttu-id="9cde6-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="9cde6-170">Response</span></span>
<span data-ttu-id="9cde6-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9cde6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





