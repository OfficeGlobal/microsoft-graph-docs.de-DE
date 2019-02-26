---
title: Erstellen von „windowsDefenderAdvancedThreatProtectionConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92afe2c99b1345fb1d987f80e8b97e3f62e74914
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258037"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="bb3e2-103">Erstellen von „windowsDefenderAdvancedThreatProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="bb3e2-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="bb3e2-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bb3e2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb3e2-105">Diese Methode erstellt ein neues Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb3e2-105">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb3e2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bb3e2-106">Prerequisites</span></span>
<span data-ttu-id="bb3e2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb3e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bb3e2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bb3e2-109">Permission type</span></span>|<span data-ttu-id="bb3e2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bb3e2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb3e2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bb3e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb3e2-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb3e2-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bb3e2-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bb3e2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb3e2-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb3e2-114">Not supported.</span></span>|
|<span data-ttu-id="bb3e2-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bb3e2-115">Application</span></span>|<span data-ttu-id="bb3e2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb3e2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb3e2-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb3e2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="bb3e2-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bb3e2-118">Request headers</span></span>
|<span data-ttu-id="bb3e2-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bb3e2-119">Header</span></span>|<span data-ttu-id="bb3e2-120">Wert</span><span class="sxs-lookup"><span data-stu-id="bb3e2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb3e2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb3e2-121">Authorization</span></span>|<span data-ttu-id="bb3e2-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bb3e2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb3e2-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bb3e2-123">Accept</span></span>|<span data-ttu-id="bb3e2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb3e2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb3e2-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bb3e2-125">Request body</span></span>
<span data-ttu-id="bb3e2-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „windowsDefenderAdvancedThreatProtectionConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="bb3e2-126">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="bb3e2-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „windowsDefenderAdvancedThreatProtectionConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="bb3e2-127">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="bb3e2-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bb3e2-128">Property</span></span>|<span data-ttu-id="bb3e2-129">Typ</span><span class="sxs-lookup"><span data-stu-id="bb3e2-129">Type</span></span>|<span data-ttu-id="bb3e2-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb3e2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb3e2-131">id</span><span class="sxs-lookup"><span data-stu-id="bb3e2-131">id</span></span>|<span data-ttu-id="bb3e2-132">string</span><span class="sxs-lookup"><span data-stu-id="bb3e2-132">String</span></span>|<span data-ttu-id="bb3e2-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bb3e2-133">Key of the entity.</span></span> <span data-ttu-id="bb3e2-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb3e2-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb3e2-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb3e2-135">lastModifiedDateTime</span></span>|<span data-ttu-id="bb3e2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb3e2-136">DateTimeOffset</span></span>|<span data-ttu-id="bb3e2-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bb3e2-137">DateTime the object was last modified.</span></span> <span data-ttu-id="bb3e2-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb3e2-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb3e2-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb3e2-139">createdDateTime</span></span>|<span data-ttu-id="bb3e2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb3e2-140">DateTimeOffset</span></span>|<span data-ttu-id="bb3e2-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="bb3e2-141">DateTime the object was created.</span></span> <span data-ttu-id="bb3e2-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb3e2-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb3e2-143">description</span><span class="sxs-lookup"><span data-stu-id="bb3e2-143">description</span></span>|<span data-ttu-id="bb3e2-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb3e2-144">String</span></span>|<span data-ttu-id="bb3e2-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bb3e2-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bb3e2-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb3e2-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb3e2-147">displayName</span><span class="sxs-lookup"><span data-stu-id="bb3e2-147">displayName</span></span>|<span data-ttu-id="bb3e2-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bb3e2-148">String</span></span>|<span data-ttu-id="bb3e2-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="bb3e2-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bb3e2-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bb3e2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb3e2-151">Version</span><span class="sxs-lookup"><span data-stu-id="bb3e2-151">version</span></span>|<span data-ttu-id="bb3e2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="bb3e2-152">Int32</span></span>|<span data-ttu-id="bb3e2-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="bb3e2-153">Version of the device configuration.</span></span> <span data-ttu-id="bb3e2-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bb3e2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bb3e2-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="bb3e2-155">allowSampleSharing</span></span>|<span data-ttu-id="bb3e2-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb3e2-156">Boolean</span></span>|<span data-ttu-id="bb3e2-157">Regel „Beispielfreigabe zulassen“ in Windows Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="bb3e2-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="bb3e2-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="bb3e2-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="bb3e2-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb3e2-159">Boolean</span></span>|<span data-ttu-id="bb3e2-160">Verkürzt das Meldungsintervall für Windows Defender Advanced Threat Protection-Telemetriedaten.</span><span class="sxs-lookup"><span data-stu-id="bb3e2-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="bb3e2-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb3e2-161">Response</span></span>
<span data-ttu-id="bb3e2-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bb3e2-162">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb3e2-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bb3e2-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb3e2-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb3e2-164">Request</span></span>
<span data-ttu-id="bb3e2-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bb3e2-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb3e2-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb3e2-166">Response</span></span>
<span data-ttu-id="bb3e2-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb3e2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



