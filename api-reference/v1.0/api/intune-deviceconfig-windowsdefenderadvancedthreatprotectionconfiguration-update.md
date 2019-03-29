---
title: Aktualisieren von „windowsDefenderAdvancedThreatProtectionConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs windowsDefenderAdvancedThreatProtectionConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1c4130b453cd2d18ee788afb4dcddc797be2719
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958767"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="5b96a-103">Aktualisieren von „windowsDefenderAdvancedThreatProtectionConfiguration“</span><span class="sxs-lookup"><span data-stu-id="5b96a-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="5b96a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="5b96a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b96a-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b96a-105">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b96a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5b96a-106">Prerequisites</span></span>
<span data-ttu-id="5b96a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b96a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b96a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b96a-109">Permission type</span></span>|<span data-ttu-id="5b96a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b96a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b96a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b96a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5b96a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b96a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b96a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b96a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b96a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b96a-114">Not supported.</span></span>|
|<span data-ttu-id="5b96a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b96a-115">Application</span></span>|<span data-ttu-id="5b96a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b96a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b96a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b96a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5b96a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b96a-118">Request headers</span></span>
|<span data-ttu-id="5b96a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5b96a-119">Header</span></span>|<span data-ttu-id="5b96a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="5b96a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b96a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b96a-121">Authorization</span></span>|<span data-ttu-id="5b96a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5b96a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b96a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5b96a-123">Accept</span></span>|<span data-ttu-id="5b96a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5b96a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b96a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b96a-125">Request body</span></span>
<span data-ttu-id="5b96a-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="5b96a-126">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="5b96a-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="5b96a-127">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="5b96a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5b96a-128">Property</span></span>|<span data-ttu-id="5b96a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="5b96a-129">Type</span></span>|<span data-ttu-id="5b96a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b96a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b96a-131">id</span><span class="sxs-lookup"><span data-stu-id="5b96a-131">id</span></span>|<span data-ttu-id="5b96a-132">String</span><span class="sxs-lookup"><span data-stu-id="5b96a-132">String</span></span>|<span data-ttu-id="5b96a-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="5b96a-133">Key of the entity.</span></span> <span data-ttu-id="5b96a-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b96a-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b96a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b96a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="5b96a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b96a-136">DateTimeOffset</span></span>|<span data-ttu-id="5b96a-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5b96a-137">DateTime the object was last modified.</span></span> <span data-ttu-id="5b96a-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b96a-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b96a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b96a-139">createdDateTime</span></span>|<span data-ttu-id="5b96a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b96a-140">DateTimeOffset</span></span>|<span data-ttu-id="5b96a-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="5b96a-141">DateTime the object was created.</span></span> <span data-ttu-id="5b96a-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b96a-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b96a-143">description</span><span class="sxs-lookup"><span data-stu-id="5b96a-143">description</span></span>|<span data-ttu-id="5b96a-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5b96a-144">String</span></span>|<span data-ttu-id="5b96a-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5b96a-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5b96a-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b96a-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b96a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="5b96a-147">displayName</span></span>|<span data-ttu-id="5b96a-148">String</span><span class="sxs-lookup"><span data-stu-id="5b96a-148">String</span></span>|<span data-ttu-id="5b96a-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="5b96a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5b96a-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b96a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b96a-151">Version</span><span class="sxs-lookup"><span data-stu-id="5b96a-151">version</span></span>|<span data-ttu-id="5b96a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="5b96a-152">Int32</span></span>|<span data-ttu-id="5b96a-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="5b96a-153">Version of the device configuration.</span></span> <span data-ttu-id="5b96a-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b96a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b96a-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="5b96a-155">allowSampleSharing</span></span>|<span data-ttu-id="5b96a-156">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="5b96a-156">Boolean</span></span>|<span data-ttu-id="5b96a-157">Regel „Beispielfreigabe zulassen“ in Windows Defender Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="5b96a-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="5b96a-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="5b96a-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="5b96a-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b96a-159">Boolean</span></span>|<span data-ttu-id="5b96a-160">Verkürzt das Meldungsintervall für Windows Defender Advanced Threat Protection-Telemetriedaten.</span><span class="sxs-lookup"><span data-stu-id="5b96a-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="5b96a-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b96a-161">Response</span></span>
<span data-ttu-id="5b96a-162">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5b96a-162">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b96a-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b96a-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b96a-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b96a-164">Request</span></span>
<span data-ttu-id="5b96a-165">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b96a-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="5b96a-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b96a-166">Response</span></span>
<span data-ttu-id="5b96a-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b96a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



