---
title: Aktualisieren von „iosCustomConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbd8c85281930c1f8d646425bcac47322802ccbb
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259017"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="a0e17-103">Aktualisieren von „iosCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="a0e17-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="a0e17-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a0e17-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0e17-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0e17-105">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0e17-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a0e17-106">Prerequisites</span></span>
<span data-ttu-id="a0e17-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a0e17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a0e17-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a0e17-109">Permission type</span></span>|<span data-ttu-id="a0e17-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a0e17-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0e17-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a0e17-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a0e17-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0e17-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0e17-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a0e17-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0e17-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0e17-114">Not supported.</span></span>|
|<span data-ttu-id="a0e17-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a0e17-115">Application</span></span>|<span data-ttu-id="a0e17-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a0e17-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0e17-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0e17-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a0e17-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a0e17-118">Request headers</span></span>
|<span data-ttu-id="a0e17-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a0e17-119">Header</span></span>|<span data-ttu-id="a0e17-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a0e17-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0e17-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0e17-121">Authorization</span></span>|<span data-ttu-id="a0e17-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a0e17-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0e17-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a0e17-123">Accept</span></span>|<span data-ttu-id="a0e17-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a0e17-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0e17-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a0e17-125">Request body</span></span>
<span data-ttu-id="a0e17-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="a0e17-126">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="a0e17-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="a0e17-127">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="a0e17-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a0e17-128">Property</span></span>|<span data-ttu-id="a0e17-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a0e17-129">Type</span></span>|<span data-ttu-id="a0e17-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a0e17-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0e17-131">id</span><span class="sxs-lookup"><span data-stu-id="a0e17-131">id</span></span>|<span data-ttu-id="a0e17-132">string</span><span class="sxs-lookup"><span data-stu-id="a0e17-132">String</span></span>|<span data-ttu-id="a0e17-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a0e17-133">Key of the entity.</span></span> <span data-ttu-id="a0e17-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0e17-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0e17-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0e17-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a0e17-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0e17-136">DateTimeOffset</span></span>|<span data-ttu-id="a0e17-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a0e17-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a0e17-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0e17-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0e17-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0e17-139">createdDateTime</span></span>|<span data-ttu-id="a0e17-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0e17-140">DateTimeOffset</span></span>|<span data-ttu-id="a0e17-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a0e17-141">DateTime the object was created.</span></span> <span data-ttu-id="a0e17-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0e17-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0e17-143">description</span><span class="sxs-lookup"><span data-stu-id="a0e17-143">description</span></span>|<span data-ttu-id="a0e17-144">String</span><span class="sxs-lookup"><span data-stu-id="a0e17-144">String</span></span>|<span data-ttu-id="a0e17-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a0e17-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a0e17-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0e17-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0e17-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a0e17-147">displayName</span></span>|<span data-ttu-id="a0e17-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0e17-148">String</span></span>|<span data-ttu-id="a0e17-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a0e17-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a0e17-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0e17-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0e17-151">Version</span><span class="sxs-lookup"><span data-stu-id="a0e17-151">version</span></span>|<span data-ttu-id="a0e17-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a0e17-152">Int32</span></span>|<span data-ttu-id="a0e17-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a0e17-153">Version of the device configuration.</span></span> <span data-ttu-id="a0e17-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a0e17-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0e17-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="a0e17-155">payloadName</span></span>|<span data-ttu-id="a0e17-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0e17-156">String</span></span>|<span data-ttu-id="a0e17-157">Name, der dem Benutzer angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="a0e17-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="a0e17-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="a0e17-158">payloadFileName</span></span>|<span data-ttu-id="a0e17-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a0e17-159">String</span></span>|<span data-ttu-id="a0e17-160">Name der Nutzlastdatei (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="a0e17-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="a0e17-161">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="a0e17-161">\*.xml).</span></span>|
|<span data-ttu-id="a0e17-162">payload</span><span class="sxs-lookup"><span data-stu-id="a0e17-162">payload</span></span>|<span data-ttu-id="a0e17-163">Binär</span><span class="sxs-lookup"><span data-stu-id="a0e17-163">Binary</span></span>|<span data-ttu-id="a0e17-164">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="a0e17-164">Payload.</span></span> <span data-ttu-id="a0e17-165">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="a0e17-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="a0e17-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0e17-166">Response</span></span>
<span data-ttu-id="a0e17-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a0e17-167">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0e17-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a0e17-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0e17-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a0e17-169">Request</span></span>
<span data-ttu-id="a0e17-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a0e17-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="a0e17-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="a0e17-171">Response</span></span>
<span data-ttu-id="a0e17-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a0e17-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



