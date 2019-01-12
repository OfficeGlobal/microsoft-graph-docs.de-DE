---
title: Aktualisieren von „macOSCustomConfiguration“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 85cd36e4df987cf4d91ed06258ee4fbd97a70cbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962534"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="7d07b-103">Aktualisieren von „macOSCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="7d07b-103">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="7d07b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7d07b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d07b-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d07b-105">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d07b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7d07b-106">Prerequisites</span></span>
<span data-ttu-id="7d07b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d07b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d07b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7d07b-109">Permission type</span></span>|<span data-ttu-id="7d07b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7d07b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d07b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7d07b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d07b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d07b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d07b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7d07b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d07b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d07b-114">Not supported.</span></span>|
|<span data-ttu-id="7d07b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7d07b-115">Application</span></span>|<span data-ttu-id="7d07b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d07b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d07b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d07b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7d07b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7d07b-118">Request headers</span></span>
|<span data-ttu-id="7d07b-119">Header</span><span class="sxs-lookup"><span data-stu-id="7d07b-119">Header</span></span>|<span data-ttu-id="7d07b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7d07b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d07b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d07b-121">Authorization</span></span>|<span data-ttu-id="7d07b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7d07b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d07b-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7d07b-123">Accept</span></span>|<span data-ttu-id="7d07b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7d07b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d07b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7d07b-125">Request body</span></span>
<span data-ttu-id="7d07b-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) an.</span><span class="sxs-lookup"><span data-stu-id="7d07b-126">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="7d07b-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="7d07b-127">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="7d07b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7d07b-128">Property</span></span>|<span data-ttu-id="7d07b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="7d07b-129">Type</span></span>|<span data-ttu-id="7d07b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7d07b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d07b-131">id</span><span class="sxs-lookup"><span data-stu-id="7d07b-131">id</span></span>|<span data-ttu-id="7d07b-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d07b-132">String</span></span>|<span data-ttu-id="7d07b-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="7d07b-133">Key of the entity.</span></span> <span data-ttu-id="7d07b-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d07b-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d07b-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d07b-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7d07b-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d07b-136">DateTimeOffset</span></span>|<span data-ttu-id="7d07b-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7d07b-137">DateTime the object was last modified.</span></span> <span data-ttu-id="7d07b-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d07b-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d07b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d07b-139">createdDateTime</span></span>|<span data-ttu-id="7d07b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d07b-140">DateTimeOffset</span></span>|<span data-ttu-id="7d07b-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="7d07b-141">DateTime the object was created.</span></span> <span data-ttu-id="7d07b-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d07b-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d07b-143">description</span><span class="sxs-lookup"><span data-stu-id="7d07b-143">description</span></span>|<span data-ttu-id="7d07b-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d07b-144">String</span></span>|<span data-ttu-id="7d07b-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7d07b-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7d07b-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d07b-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d07b-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7d07b-147">displayName</span></span>|<span data-ttu-id="7d07b-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d07b-148">String</span></span>|<span data-ttu-id="7d07b-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="7d07b-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7d07b-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d07b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d07b-151">Version</span><span class="sxs-lookup"><span data-stu-id="7d07b-151">version</span></span>|<span data-ttu-id="7d07b-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7d07b-152">Int32</span></span>|<span data-ttu-id="7d07b-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="7d07b-153">Version of the device configuration.</span></span> <span data-ttu-id="7d07b-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7d07b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d07b-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="7d07b-155">payloadName</span></span>|<span data-ttu-id="7d07b-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d07b-156">String</span></span>|<span data-ttu-id="7d07b-157">Name, der dem Benutzer angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="7d07b-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="7d07b-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="7d07b-158">payloadFileName</span></span>|<span data-ttu-id="7d07b-159">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7d07b-159">String</span></span>|<span data-ttu-id="7d07b-160">Name der Nutzlastdatei (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="7d07b-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="7d07b-161">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="7d07b-161">\*.xml).</span></span>|
|<span data-ttu-id="7d07b-162">payload</span><span class="sxs-lookup"><span data-stu-id="7d07b-162">payload</span></span>|<span data-ttu-id="7d07b-163">Binär</span><span class="sxs-lookup"><span data-stu-id="7d07b-163">Binary</span></span>|<span data-ttu-id="7d07b-164">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="7d07b-164">Payload.</span></span> <span data-ttu-id="7d07b-165">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="7d07b-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="7d07b-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d07b-166">Response</span></span>
<span data-ttu-id="7d07b-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7d07b-167">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d07b-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7d07b-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d07b-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d07b-169">Request</span></span>
<span data-ttu-id="7d07b-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7d07b-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d07b-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d07b-171">Response</span></span>
<span data-ttu-id="7d07b-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7d07b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



