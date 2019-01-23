---
title: Erstellen von deviceManagementScript
description: Erstellen eines neuen DeviceManagementScript-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be0ffb8b912b25684ba0ed3dc383a995fb872f3b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409272"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="f06e8-103">Erstellen von deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="f06e8-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="f06e8-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f06e8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f06e8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f06e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f06e8-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f06e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f06e8-107">Erstellen eines neuen [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="f06e8-107">Create a new [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f06e8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f06e8-108">Prerequisites</span></span>
<span data-ttu-id="f06e8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f06e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f06e8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f06e8-111">Permission type</span></span>|<span data-ttu-id="f06e8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f06e8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f06e8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f06e8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f06e8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f06e8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f06e8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f06e8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f06e8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f06e8-116">Not supported.</span></span>|
|<span data-ttu-id="f06e8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f06e8-117">Application</span></span>|<span data-ttu-id="f06e8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f06e8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f06e8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f06e8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="f06e8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f06e8-120">Request headers</span></span>
|<span data-ttu-id="f06e8-121">Header</span><span class="sxs-lookup"><span data-stu-id="f06e8-121">Header</span></span>|<span data-ttu-id="f06e8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f06e8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f06e8-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f06e8-123">Authorization</span></span>|<span data-ttu-id="f06e8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f06e8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f06e8-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f06e8-125">Accept</span></span>|<span data-ttu-id="f06e8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f06e8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f06e8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f06e8-127">Request body</span></span>
<span data-ttu-id="f06e8-128">Geben Sie im Textkörper Anforderung für das Objekt DeviceManagementScript eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="f06e8-128">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="f06e8-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die DeviceManagementScript erstellen.</span><span class="sxs-lookup"><span data-stu-id="f06e8-129">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="f06e8-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f06e8-130">Property</span></span>|<span data-ttu-id="f06e8-131">Typ</span><span class="sxs-lookup"><span data-stu-id="f06e8-131">Type</span></span>|<span data-ttu-id="f06e8-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f06e8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f06e8-133">id</span><span class="sxs-lookup"><span data-stu-id="f06e8-133">id</span></span>|<span data-ttu-id="f06e8-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f06e8-134">String</span></span>|<span data-ttu-id="f06e8-135">Eindeutiger Bezeichner für das Gerät Management-Skript.</span><span class="sxs-lookup"><span data-stu-id="f06e8-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="f06e8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f06e8-136">displayName</span></span>|<span data-ttu-id="f06e8-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f06e8-137">String</span></span>|<span data-ttu-id="f06e8-138">Name des Skripts Management Gerät.</span><span class="sxs-lookup"><span data-stu-id="f06e8-138">Name of the device management script.</span></span>|
|<span data-ttu-id="f06e8-139">description</span><span class="sxs-lookup"><span data-stu-id="f06e8-139">description</span></span>|<span data-ttu-id="f06e8-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f06e8-140">String</span></span>|<span data-ttu-id="f06e8-141">Optionale Beschreibung für das Gerät Management-Skript.</span><span class="sxs-lookup"><span data-stu-id="f06e8-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="f06e8-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="f06e8-142">runSchedule</span></span>|[<span data-ttu-id="f06e8-143">runSchedule</span><span class="sxs-lookup"><span data-stu-id="f06e8-143">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="f06e8-144">Das Intervall für das Skript ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="f06e8-144">The interval for script to run.</span></span> <span data-ttu-id="f06e8-145">Wenn nicht definiert das Skript einmal ausgeführt wird</span><span class="sxs-lookup"><span data-stu-id="f06e8-145">If not defined the script will run once</span></span>|
|<span data-ttu-id="f06e8-146">scriptContent</span><span class="sxs-lookup"><span data-stu-id="f06e8-146">scriptContent</span></span>|<span data-ttu-id="f06e8-147">Binär</span><span class="sxs-lookup"><span data-stu-id="f06e8-147">Binary</span></span>|<span data-ttu-id="f06e8-148">Der Skriptinhalt.</span><span class="sxs-lookup"><span data-stu-id="f06e8-148">The script content.</span></span>|
|<span data-ttu-id="f06e8-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f06e8-149">createdDateTime</span></span>|<span data-ttu-id="f06e8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f06e8-150">DateTimeOffset</span></span>|<span data-ttu-id="f06e8-151">Datum und Zeit für das Gerät Management-Skript erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="f06e8-151">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="f06e8-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f06e8-152">lastModifiedDateTime</span></span>|<span data-ttu-id="f06e8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f06e8-153">DateTimeOffset</span></span>|<span data-ttu-id="f06e8-154">Datum und Uhrzeit der letzten Änderung des Geräts Management-Skripts.</span><span class="sxs-lookup"><span data-stu-id="f06e8-154">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="f06e8-155">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="f06e8-155">runAsAccount</span></span>|[<span data-ttu-id="f06e8-156">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="f06e8-156">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="f06e8-157">Gibt den Typ des Ausführungskontexts, den das Gerät Management-Skript in ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="f06e8-157">Indicates the type of execution context the device management script runs in.</span></span> <span data-ttu-id="f06e8-158">Mögliche Werte sind: `system` und `user`.</span><span class="sxs-lookup"><span data-stu-id="f06e8-158">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="f06e8-159">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="f06e8-159">enforceSignatureCheck</span></span>|<span data-ttu-id="f06e8-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f06e8-160">Boolean</span></span>|<span data-ttu-id="f06e8-161">Geben Sie an, ob die Signatur Skript muss aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="f06e8-161">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="f06e8-162">fileName</span><span class="sxs-lookup"><span data-stu-id="f06e8-162">fileName</span></span>|<span data-ttu-id="f06e8-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f06e8-163">String</span></span>|<span data-ttu-id="f06e8-164">Dateiname des Skripts.</span><span class="sxs-lookup"><span data-stu-id="f06e8-164">Script file name.</span></span>|
|<span data-ttu-id="f06e8-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f06e8-165">roleScopeTagIds</span></span>|<span data-ttu-id="f06e8-166">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="f06e8-166">String collection</span></span>|<span data-ttu-id="f06e8-167">Liste der Bereichs-Tag-IDs für diese Instanz des PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="f06e8-167">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="f06e8-168">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="f06e8-168">runAs32Bit</span></span>|<span data-ttu-id="f06e8-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="f06e8-169">Boolean</span></span>|<span data-ttu-id="f06e8-170">Ein Wert, der angibt, ob das PowerShell-Skript als 32-Bit ausgeführt werden soll</span><span class="sxs-lookup"><span data-stu-id="f06e8-170">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="f06e8-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="f06e8-171">Response</span></span>
<span data-ttu-id="f06e8-172">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="f06e8-172">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f06e8-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f06e8-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="f06e8-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f06e8-174">Request</span></span>
<span data-ttu-id="f06e8-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f06e8-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f06e8-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="f06e8-176">Response</span></span>
<span data-ttu-id="f06e8-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f06e8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




