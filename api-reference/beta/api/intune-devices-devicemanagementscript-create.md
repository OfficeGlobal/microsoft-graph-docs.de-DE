---
title: Devicemanagementscript hinzugefügt erstellen
description: Erstellen eines neuen Devicemanagementscript hinzugefügt-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 40472e27f1ba900121c5c7927ec5d15f27582c99
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173619"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="d4c5a-103">Devicemanagementscript hinzugefügt erstellen</span><span class="sxs-lookup"><span data-stu-id="d4c5a-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="d4c5a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4c5a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4c5a-106">Erstellen eines neuen [devicemanagementscript hinzugefügt](../resources/intune-devices-devicemanagementscript.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-106">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4c5a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d4c5a-107">Prerequisites</span></span>
<span data-ttu-id="d4c5a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d4c5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d4c5a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d4c5a-110">Permission type</span></span>|<span data-ttu-id="d4c5a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d4c5a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4c5a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d4c5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4c5a-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4c5a-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d4c5a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d4c5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4c5a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4c5a-115">Not supported.</span></span>|
|<span data-ttu-id="d4c5a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d4c5a-116">Application</span></span>|<span data-ttu-id="d4c5a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d4c5a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4c5a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4c5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="d4c5a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d4c5a-119">Request headers</span></span>
|<span data-ttu-id="d4c5a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d4c5a-120">Header</span></span>|<span data-ttu-id="d4c5a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d4c5a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4c5a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4c5a-122">Authorization</span></span>|<span data-ttu-id="d4c5a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d4c5a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4c5a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d4c5a-124">Accept</span></span>|<span data-ttu-id="d4c5a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4c5a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4c5a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d4c5a-126">Request body</span></span>
<span data-ttu-id="d4c5a-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das Devicemanagementscript hinzugefügt-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-127">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="d4c5a-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der Devicemanagementscript hinzugefügt erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-128">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="d4c5a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d4c5a-129">Property</span></span>|<span data-ttu-id="d4c5a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d4c5a-130">Type</span></span>|<span data-ttu-id="d4c5a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d4c5a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4c5a-132">id</span><span class="sxs-lookup"><span data-stu-id="d4c5a-132">id</span></span>|<span data-ttu-id="d4c5a-133">string</span><span class="sxs-lookup"><span data-stu-id="d4c5a-133">String</span></span>|<span data-ttu-id="d4c5a-134">Eindeutiger Bezeichner für das Geräte Verwaltungsskript.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="d4c5a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d4c5a-135">displayName</span></span>|<span data-ttu-id="d4c5a-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4c5a-136">String</span></span>|<span data-ttu-id="d4c5a-137">Name des Geräteverwaltungs-Skripts.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-137">Name of the device management script.</span></span>|
|<span data-ttu-id="d4c5a-138">description</span><span class="sxs-lookup"><span data-stu-id="d4c5a-138">description</span></span>|<span data-ttu-id="d4c5a-139">String</span><span class="sxs-lookup"><span data-stu-id="d4c5a-139">String</span></span>|<span data-ttu-id="d4c5a-140">Optionale Beschreibung des Device Management-Skripts.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="d4c5a-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="d4c5a-141">runSchedule</span></span>|[<span data-ttu-id="d4c5a-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="d4c5a-142">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="d4c5a-143">Das Intervall für die Ausführung des Skripts.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-143">The interval for script to run.</span></span> <span data-ttu-id="d4c5a-144">Wenn nicht definiert, wird das Skript einmal ausgeführt</span><span class="sxs-lookup"><span data-stu-id="d4c5a-144">If not defined the script will run once</span></span>|
|<span data-ttu-id="d4c5a-145">scriptContent</span><span class="sxs-lookup"><span data-stu-id="d4c5a-145">scriptContent</span></span>|<span data-ttu-id="d4c5a-146">Binär</span><span class="sxs-lookup"><span data-stu-id="d4c5a-146">Binary</span></span>|<span data-ttu-id="d4c5a-147">Der Skriptinhalt.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-147">The script content.</span></span>|
|<span data-ttu-id="d4c5a-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4c5a-148">createdDateTime</span></span>|<span data-ttu-id="d4c5a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4c5a-149">DateTimeOffset</span></span>|<span data-ttu-id="d4c5a-150">Das Datum und die Uhrzeit, zu der das Geräte Verwaltungsskript erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-150">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="d4c5a-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4c5a-151">lastModifiedDateTime</span></span>|<span data-ttu-id="d4c5a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4c5a-152">DateTimeOffset</span></span>|<span data-ttu-id="d4c5a-153">Datum und Uhrzeit der letzten Änderung des Geräteverwaltungsskripts.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-153">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="d4c5a-154">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="d4c5a-154">runAsAccount</span></span>|[<span data-ttu-id="d4c5a-155">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="d4c5a-155">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="d4c5a-156">Gibt den Typ des Ausführungskontexts an, in dem das Geräte Verwaltungsskript ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-156">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="d4c5a-157">Mögliche Werte sind: `system` und `user`.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-157">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="d4c5a-158">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="d4c5a-158">enforceSignatureCheck</span></span>|<span data-ttu-id="d4c5a-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4c5a-159">Boolean</span></span>|<span data-ttu-id="d4c5a-160">Geben Sie an, ob die skriptsignatur überprüft werden muss.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-160">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="d4c5a-161">fileName</span><span class="sxs-lookup"><span data-stu-id="d4c5a-161">fileName</span></span>|<span data-ttu-id="d4c5a-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d4c5a-162">String</span></span>|<span data-ttu-id="d4c5a-163">Skriptdateiname.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-163">Script file name.</span></span>|
|<span data-ttu-id="d4c5a-164">Rolescopetagids zur</span><span class="sxs-lookup"><span data-stu-id="d4c5a-164">roleScopeTagIds</span></span>|<span data-ttu-id="d4c5a-165">String collection</span><span class="sxs-lookup"><span data-stu-id="d4c5a-165">String collection</span></span>|<span data-ttu-id="d4c5a-166">Liste der Bereichstag-IDs für diese PowerShellScript-Instanz.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-166">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="d4c5a-167">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="d4c5a-167">runAs32Bit</span></span>|<span data-ttu-id="d4c5a-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4c5a-168">Boolean</span></span>|<span data-ttu-id="d4c5a-169">Ein Wert, der angibt, ob das PowerShell-Skript als 32-Bit ausgeführt werden soll</span><span class="sxs-lookup"><span data-stu-id="d4c5a-169">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="d4c5a-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4c5a-170">Response</span></span>
<span data-ttu-id="d4c5a-171">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [devicemanagementscript hinzugefügt](../resources/intune-devices-devicemanagementscript.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-171">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4c5a-172">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d4c5a-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4c5a-173">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d4c5a-173">Request</span></span>
<span data-ttu-id="d4c5a-174">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```

### <a name="response"></a><span data-ttu-id="d4c5a-175">Antwort</span><span class="sxs-lookup"><span data-stu-id="d4c5a-175">Response</span></span>
<span data-ttu-id="d4c5a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d4c5a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 615

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
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```




