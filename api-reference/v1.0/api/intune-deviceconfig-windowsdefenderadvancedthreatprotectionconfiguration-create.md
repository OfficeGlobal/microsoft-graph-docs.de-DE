---
title: Erstellen von „windowsDefenderAdvancedThreatProtectionConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windowsDefenderAdvancedThreatProtectionConfiguration.
ms.openlocfilehash: 84de15adc3178ae13530ba43c8361f636573f30b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017638"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="06015-103">Erstellen von „windowsDefenderAdvancedThreatProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="06015-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="06015-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="06015-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="06015-105">Diese Methode erstellt ein neues Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06015-105">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="06015-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="06015-106">Prerequisites</span></span>
<span data-ttu-id="06015-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06015-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06015-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06015-109">Permission type</span></span>|<span data-ttu-id="06015-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06015-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06015-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06015-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06015-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06015-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="06015-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06015-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06015-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06015-114">Not supported.</span></span>|
|<span data-ttu-id="06015-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06015-115">Application</span></span>|<span data-ttu-id="06015-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="06015-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06015-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06015-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="06015-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06015-118">Request headers</span></span>
|<span data-ttu-id="06015-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="06015-119">Header</span></span>|<span data-ttu-id="06015-120">Wert</span><span class="sxs-lookup"><span data-stu-id="06015-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06015-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="06015-121">Authorization</span></span>|<span data-ttu-id="06015-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="06015-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06015-123">Accept</span><span class="sxs-lookup"><span data-stu-id="06015-123">Accept</span></span>|<span data-ttu-id="06015-124">application/json</span><span class="sxs-lookup"><span data-stu-id="06015-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06015-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06015-125">Request body</span></span>
<span data-ttu-id="06015-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsDefenderAdvancedThreatProtectionConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="06015-126">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="06015-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsDefenderAdvancedThreatProtectionConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="06015-127">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="06015-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="06015-128">Property</span></span>|<span data-ttu-id="06015-129">Typ</span><span class="sxs-lookup"><span data-stu-id="06015-129">Type</span></span>|<span data-ttu-id="06015-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="06015-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06015-131">id</span><span class="sxs-lookup"><span data-stu-id="06015-131">id</span></span>|<span data-ttu-id="06015-132">String</span><span class="sxs-lookup"><span data-stu-id="06015-132">String</span></span>|<span data-ttu-id="06015-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="06015-133">Key of the entity.</span></span> <span data-ttu-id="06015-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06015-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06015-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="06015-135">lastModifiedDateTime</span></span>|<span data-ttu-id="06015-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06015-136">DateTimeOffset</span></span>|<span data-ttu-id="06015-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="06015-137">DateTime the object was last modified.</span></span> <span data-ttu-id="06015-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06015-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06015-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="06015-139">createdDateTime</span></span>|<span data-ttu-id="06015-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06015-140">DateTimeOffset</span></span>|<span data-ttu-id="06015-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="06015-141">DateTime the object was created.</span></span> <span data-ttu-id="06015-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06015-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06015-143">description</span><span class="sxs-lookup"><span data-stu-id="06015-143">description</span></span>|<span data-ttu-id="06015-144">String</span><span class="sxs-lookup"><span data-stu-id="06015-144">String</span></span>|<span data-ttu-id="06015-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="06015-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="06015-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06015-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06015-147">displayName</span><span class="sxs-lookup"><span data-stu-id="06015-147">displayName</span></span>|<span data-ttu-id="06015-148">String</span><span class="sxs-lookup"><span data-stu-id="06015-148">String</span></span>|<span data-ttu-id="06015-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="06015-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="06015-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06015-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06015-151">Version</span><span class="sxs-lookup"><span data-stu-id="06015-151">version</span></span>|<span data-ttu-id="06015-152">Int32</span><span class="sxs-lookup"><span data-stu-id="06015-152">Int32</span></span>|<span data-ttu-id="06015-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="06015-153">Version of the device configuration.</span></span> <span data-ttu-id="06015-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="06015-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="06015-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="06015-155">allowSampleSharing</span></span>|<span data-ttu-id="06015-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06015-156">Boolean</span></span>|<span data-ttu-id="06015-157">Regel „Beispielfreigabe zulassen“ in Windows Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="06015-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="06015-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="06015-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="06015-159">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="06015-159">Boolean</span></span>|<span data-ttu-id="06015-160">Verkürzt das Meldungsintervall für Windows Defender Advanced Threat Protection-Telemetriedaten.</span><span class="sxs-lookup"><span data-stu-id="06015-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="06015-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="06015-161">Response</span></span>
<span data-ttu-id="06015-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="06015-162">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06015-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06015-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="06015-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06015-164">Request</span></span>
<span data-ttu-id="06015-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06015-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="06015-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="06015-166">Response</span></span>
<span data-ttu-id="06015-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06015-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```


