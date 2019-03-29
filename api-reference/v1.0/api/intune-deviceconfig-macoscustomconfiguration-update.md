---
title: Aktualisieren von „macOSCustomConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b8895014666e4c75e885ad9ee529ae1faa1a40c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977975"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="52e33-103">Aktualisieren von „macOSCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="52e33-103">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="52e33-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="52e33-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52e33-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52e33-105">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52e33-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="52e33-106">Prerequisites</span></span>
<span data-ttu-id="52e33-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52e33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52e33-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="52e33-109">Permission type</span></span>|<span data-ttu-id="52e33-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="52e33-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52e33-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="52e33-111">Delegated (work or school account)</span></span>|<span data-ttu-id="52e33-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52e33-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="52e33-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="52e33-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52e33-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52e33-114">Not supported.</span></span>|
|<span data-ttu-id="52e33-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="52e33-115">Application</span></span>|<span data-ttu-id="52e33-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="52e33-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52e33-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="52e33-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="52e33-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="52e33-118">Request headers</span></span>
|<span data-ttu-id="52e33-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="52e33-119">Header</span></span>|<span data-ttu-id="52e33-120">Wert</span><span class="sxs-lookup"><span data-stu-id="52e33-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52e33-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="52e33-121">Authorization</span></span>|<span data-ttu-id="52e33-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="52e33-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52e33-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="52e33-123">Accept</span></span>|<span data-ttu-id="52e33-124">application/json</span><span class="sxs-lookup"><span data-stu-id="52e33-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52e33-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="52e33-125">Request body</span></span>
<span data-ttu-id="52e33-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="52e33-126">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="52e33-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="52e33-127">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="52e33-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="52e33-128">Property</span></span>|<span data-ttu-id="52e33-129">Typ</span><span class="sxs-lookup"><span data-stu-id="52e33-129">Type</span></span>|<span data-ttu-id="52e33-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52e33-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52e33-131">id</span><span class="sxs-lookup"><span data-stu-id="52e33-131">id</span></span>|<span data-ttu-id="52e33-132">String</span><span class="sxs-lookup"><span data-stu-id="52e33-132">String</span></span>|<span data-ttu-id="52e33-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="52e33-133">Key of the entity.</span></span> <span data-ttu-id="52e33-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52e33-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52e33-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="52e33-135">lastModifiedDateTime</span></span>|<span data-ttu-id="52e33-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52e33-136">DateTimeOffset</span></span>|<span data-ttu-id="52e33-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="52e33-137">DateTime the object was last modified.</span></span> <span data-ttu-id="52e33-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52e33-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52e33-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52e33-139">createdDateTime</span></span>|<span data-ttu-id="52e33-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52e33-140">DateTimeOffset</span></span>|<span data-ttu-id="52e33-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="52e33-141">DateTime the object was created.</span></span> <span data-ttu-id="52e33-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52e33-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52e33-143">description</span><span class="sxs-lookup"><span data-stu-id="52e33-143">description</span></span>|<span data-ttu-id="52e33-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52e33-144">String</span></span>|<span data-ttu-id="52e33-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="52e33-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="52e33-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52e33-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52e33-147">displayName</span><span class="sxs-lookup"><span data-stu-id="52e33-147">displayName</span></span>|<span data-ttu-id="52e33-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="52e33-148">String</span></span>|<span data-ttu-id="52e33-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="52e33-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="52e33-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52e33-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52e33-151">Version</span><span class="sxs-lookup"><span data-stu-id="52e33-151">version</span></span>|<span data-ttu-id="52e33-152">Int32</span><span class="sxs-lookup"><span data-stu-id="52e33-152">Int32</span></span>|<span data-ttu-id="52e33-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="52e33-153">Version of the device configuration.</span></span> <span data-ttu-id="52e33-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="52e33-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="52e33-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="52e33-155">payloadName</span></span>|<span data-ttu-id="52e33-156">String</span><span class="sxs-lookup"><span data-stu-id="52e33-156">String</span></span>|<span data-ttu-id="52e33-157">Name, der dem Benutzer angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="52e33-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="52e33-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="52e33-158">payloadFileName</span></span>|<span data-ttu-id="52e33-159">String</span><span class="sxs-lookup"><span data-stu-id="52e33-159">String</span></span>|<span data-ttu-id="52e33-160">Name der Nutzlastdatei (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="52e33-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="52e33-161">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="52e33-161">\*.xml).</span></span>|
|<span data-ttu-id="52e33-162">payload</span><span class="sxs-lookup"><span data-stu-id="52e33-162">payload</span></span>|<span data-ttu-id="52e33-163">Binär</span><span class="sxs-lookup"><span data-stu-id="52e33-163">Binary</span></span>|<span data-ttu-id="52e33-164">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="52e33-164">Payload.</span></span> <span data-ttu-id="52e33-165">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="52e33-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="52e33-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="52e33-166">Response</span></span>
<span data-ttu-id="52e33-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="52e33-167">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52e33-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="52e33-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="52e33-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="52e33-169">Request</span></span>
<span data-ttu-id="52e33-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="52e33-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="52e33-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="52e33-171">Response</span></span>
<span data-ttu-id="52e33-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="52e33-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```



