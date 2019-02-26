---
title: Erstellen von „iosCustomConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ecdc9ca4fb9218ae77c1c144feeb4ca2cb5c389d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261614"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="4d5f9-103">Erstellen von „iosCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="4d5f9-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="4d5f9-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4d5f9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d5f9-105">Diese Methode erstellt ein neues Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d5f9-105">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d5f9-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4d5f9-106">Prerequisites</span></span>
<span data-ttu-id="4d5f9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d5f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4d5f9-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d5f9-109">Permission type</span></span>|<span data-ttu-id="4d5f9-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d5f9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d5f9-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d5f9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d5f9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d5f9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4d5f9-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d5f9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d5f9-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d5f9-114">Not supported.</span></span>|
|<span data-ttu-id="4d5f9-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d5f9-115">Application</span></span>|<span data-ttu-id="4d5f9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d5f9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d5f9-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d5f9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4d5f9-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d5f9-118">Request headers</span></span>
|<span data-ttu-id="4d5f9-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4d5f9-119">Header</span></span>|<span data-ttu-id="4d5f9-120">Wert</span><span class="sxs-lookup"><span data-stu-id="4d5f9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d5f9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d5f9-121">Authorization</span></span>|<span data-ttu-id="4d5f9-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d5f9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d5f9-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4d5f9-123">Accept</span></span>|<span data-ttu-id="4d5f9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4d5f9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d5f9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d5f9-125">Request body</span></span>
<span data-ttu-id="4d5f9-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „iosCustomConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="4d5f9-126">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="4d5f9-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „iosCustomConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="4d5f9-127">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="4d5f9-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d5f9-128">Property</span></span>|<span data-ttu-id="4d5f9-129">Typ</span><span class="sxs-lookup"><span data-stu-id="4d5f9-129">Type</span></span>|<span data-ttu-id="4d5f9-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d5f9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d5f9-131">id</span><span class="sxs-lookup"><span data-stu-id="4d5f9-131">id</span></span>|<span data-ttu-id="4d5f9-132">string</span><span class="sxs-lookup"><span data-stu-id="4d5f9-132">String</span></span>|<span data-ttu-id="4d5f9-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4d5f9-133">Key of the entity.</span></span> <span data-ttu-id="4d5f9-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d5f9-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d5f9-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d5f9-135">lastModifiedDateTime</span></span>|<span data-ttu-id="4d5f9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d5f9-136">DateTimeOffset</span></span>|<span data-ttu-id="4d5f9-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4d5f9-137">DateTime the object was last modified.</span></span> <span data-ttu-id="4d5f9-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d5f9-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d5f9-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d5f9-139">createdDateTime</span></span>|<span data-ttu-id="4d5f9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d5f9-140">DateTimeOffset</span></span>|<span data-ttu-id="4d5f9-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="4d5f9-141">DateTime the object was created.</span></span> <span data-ttu-id="4d5f9-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d5f9-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d5f9-143">description</span><span class="sxs-lookup"><span data-stu-id="4d5f9-143">description</span></span>|<span data-ttu-id="4d5f9-144">String</span><span class="sxs-lookup"><span data-stu-id="4d5f9-144">String</span></span>|<span data-ttu-id="4d5f9-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4d5f9-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4d5f9-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d5f9-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d5f9-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4d5f9-147">displayName</span></span>|<span data-ttu-id="4d5f9-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d5f9-148">String</span></span>|<span data-ttu-id="4d5f9-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="4d5f9-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4d5f9-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d5f9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d5f9-151">Version</span><span class="sxs-lookup"><span data-stu-id="4d5f9-151">version</span></span>|<span data-ttu-id="4d5f9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4d5f9-152">Int32</span></span>|<span data-ttu-id="4d5f9-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="4d5f9-153">Version of the device configuration.</span></span> <span data-ttu-id="4d5f9-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4d5f9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4d5f9-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="4d5f9-155">payloadName</span></span>|<span data-ttu-id="4d5f9-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d5f9-156">String</span></span>|<span data-ttu-id="4d5f9-157">Name, der dem Benutzer angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="4d5f9-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="4d5f9-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="4d5f9-158">payloadFileName</span></span>|<span data-ttu-id="4d5f9-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4d5f9-159">String</span></span>|<span data-ttu-id="4d5f9-160">Name der Nutzlastdatei (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="4d5f9-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="4d5f9-161">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="4d5f9-161">\*.xml).</span></span>|
|<span data-ttu-id="4d5f9-162">payload</span><span class="sxs-lookup"><span data-stu-id="4d5f9-162">payload</span></span>|<span data-ttu-id="4d5f9-163">Binär</span><span class="sxs-lookup"><span data-stu-id="4d5f9-163">Binary</span></span>|<span data-ttu-id="4d5f9-164">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="4d5f9-164">Payload.</span></span> <span data-ttu-id="4d5f9-165">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="4d5f9-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="4d5f9-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d5f9-166">Response</span></span>
<span data-ttu-id="4d5f9-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4d5f9-167">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d5f9-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d5f9-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d5f9-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d5f9-169">Request</span></span>
<span data-ttu-id="4d5f9-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d5f9-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="4d5f9-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d5f9-171">Response</span></span>
<span data-ttu-id="4d5f9-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d5f9-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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



