---
title: Erstellen von „macOSCustomConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs macOSCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 52c3e4adf4dd6c3e934d8d6ce482d1c2aeeadcde
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348804"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="a35df-103">Erstellen von „macOSCustomConfiguration“</span><span class="sxs-lookup"><span data-stu-id="a35df-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="a35df-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a35df-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a35df-105">Diese Methode erstellt ein neues Objekt des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a35df-105">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a35df-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a35df-106">Prerequisites</span></span>
<span data-ttu-id="a35df-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a35df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a35df-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a35df-109">Permission type</span></span>|<span data-ttu-id="a35df-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a35df-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a35df-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a35df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a35df-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a35df-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a35df-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a35df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a35df-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a35df-114">Not supported.</span></span>|
|<span data-ttu-id="a35df-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a35df-115">Application</span></span>|<span data-ttu-id="a35df-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a35df-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a35df-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a35df-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a35df-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a35df-118">Request headers</span></span>
|<span data-ttu-id="a35df-119">Header</span><span class="sxs-lookup"><span data-stu-id="a35df-119">Header</span></span>|<span data-ttu-id="a35df-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a35df-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a35df-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a35df-121">Authorization</span></span>|<span data-ttu-id="a35df-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a35df-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a35df-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a35df-123">Accept</span></span>|<span data-ttu-id="a35df-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a35df-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a35df-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a35df-125">Request body</span></span>
<span data-ttu-id="a35df-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „macOSCustomConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="a35df-126">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="a35df-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSCustomConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="a35df-127">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="a35df-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a35df-128">Property</span></span>|<span data-ttu-id="a35df-129">Typ</span><span class="sxs-lookup"><span data-stu-id="a35df-129">Type</span></span>|<span data-ttu-id="a35df-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a35df-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a35df-131">id</span><span class="sxs-lookup"><span data-stu-id="a35df-131">id</span></span>|<span data-ttu-id="a35df-132">String</span><span class="sxs-lookup"><span data-stu-id="a35df-132">String</span></span>|<span data-ttu-id="a35df-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="a35df-133">Key of the entity.</span></span> <span data-ttu-id="a35df-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a35df-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a35df-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a35df-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a35df-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a35df-136">DateTimeOffset</span></span>|<span data-ttu-id="a35df-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a35df-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a35df-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a35df-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a35df-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a35df-139">createdDateTime</span></span>|<span data-ttu-id="a35df-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a35df-140">DateTimeOffset</span></span>|<span data-ttu-id="a35df-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="a35df-141">DateTime the object was created.</span></span> <span data-ttu-id="a35df-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a35df-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a35df-143">description</span><span class="sxs-lookup"><span data-stu-id="a35df-143">description</span></span>|<span data-ttu-id="a35df-144">String</span><span class="sxs-lookup"><span data-stu-id="a35df-144">String</span></span>|<span data-ttu-id="a35df-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a35df-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a35df-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a35df-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a35df-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a35df-147">displayName</span></span>|<span data-ttu-id="a35df-148">String</span><span class="sxs-lookup"><span data-stu-id="a35df-148">String</span></span>|<span data-ttu-id="a35df-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="a35df-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a35df-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a35df-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a35df-151">Version</span><span class="sxs-lookup"><span data-stu-id="a35df-151">version</span></span>|<span data-ttu-id="a35df-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a35df-152">Int32</span></span>|<span data-ttu-id="a35df-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="a35df-153">Version of the device configuration.</span></span> <span data-ttu-id="a35df-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a35df-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a35df-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="a35df-155">payloadName</span></span>|<span data-ttu-id="a35df-156">String</span><span class="sxs-lookup"><span data-stu-id="a35df-156">String</span></span>|<span data-ttu-id="a35df-157">Name, der dem Benutzer angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="a35df-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="a35df-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="a35df-158">payloadFileName</span></span>|<span data-ttu-id="a35df-159">String</span><span class="sxs-lookup"><span data-stu-id="a35df-159">String</span></span>|<span data-ttu-id="a35df-160">Name der Nutzlastdatei (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="a35df-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="a35df-161">\*.xml)</span><span class="sxs-lookup"><span data-stu-id="a35df-161">\*.xml).</span></span>|
|<span data-ttu-id="a35df-162">payload</span><span class="sxs-lookup"><span data-stu-id="a35df-162">payload</span></span>|<span data-ttu-id="a35df-163">Binär</span><span class="sxs-lookup"><span data-stu-id="a35df-163">Binary</span></span>|<span data-ttu-id="a35df-164">Nutzlast</span><span class="sxs-lookup"><span data-stu-id="a35df-164">Payload.</span></span> <span data-ttu-id="a35df-165">(UTF8-codiertes Bytearray)</span><span class="sxs-lookup"><span data-stu-id="a35df-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="a35df-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="a35df-166">Response</span></span>
<span data-ttu-id="a35df-167">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a35df-167">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a35df-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a35df-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="a35df-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a35df-169">Request</span></span>
<span data-ttu-id="a35df-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a35df-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="a35df-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="a35df-171">Response</span></span>
<span data-ttu-id="a35df-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a35df-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



