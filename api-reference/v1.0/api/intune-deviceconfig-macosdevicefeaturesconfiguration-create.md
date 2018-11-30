---
title: Erstellen von „macOSDeviceFeaturesConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs macOSDeviceFeaturesConfiguration.
ms.openlocfilehash: e8d6d16ce66e512d44cbae63ec41122b526ac471
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016088"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="b4c2f-103">Erstellen von „macOSDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="b4c2f-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="b4c2f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b4c2f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4c2f-105">Diese Methode erstellt ein neues Objekt des Typs [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4c2f-105">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b4c2f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b4c2f-106">Prerequisites</span></span>
<span data-ttu-id="b4c2f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4c2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4c2f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4c2f-109">Permission type</span></span>|<span data-ttu-id="b4c2f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4c2f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4c2f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4c2f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b4c2f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4c2f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4c2f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4c2f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4c2f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4c2f-114">Not supported.</span></span>|
|<span data-ttu-id="b4c2f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4c2f-115">Application</span></span>|<span data-ttu-id="b4c2f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4c2f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4c2f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4c2f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b4c2f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4c2f-118">Request headers</span></span>
|<span data-ttu-id="b4c2f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b4c2f-119">Header</span></span>|<span data-ttu-id="b4c2f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="b4c2f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4c2f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4c2f-121">Authorization</span></span>|<span data-ttu-id="b4c2f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b4c2f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4c2f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b4c2f-123">Accept</span></span>|<span data-ttu-id="b4c2f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b4c2f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4c2f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4c2f-125">Request body</span></span>
<span data-ttu-id="b4c2f-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „macOSDeviceFeaturesConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="b4c2f-126">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="b4c2f-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSDeviceFeaturesConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="b4c2f-127">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="b4c2f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b4c2f-128">Property</span></span>|<span data-ttu-id="b4c2f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="b4c2f-129">Type</span></span>|<span data-ttu-id="b4c2f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b4c2f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4c2f-131">id</span><span class="sxs-lookup"><span data-stu-id="b4c2f-131">id</span></span>|<span data-ttu-id="b4c2f-132">String</span><span class="sxs-lookup"><span data-stu-id="b4c2f-132">String</span></span>|<span data-ttu-id="b4c2f-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b4c2f-133">Key of the entity.</span></span> <span data-ttu-id="b4c2f-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4c2f-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4c2f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4c2f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b4c2f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4c2f-136">DateTimeOffset</span></span>|<span data-ttu-id="b4c2f-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4c2f-137">DateTime the object was last modified.</span></span> <span data-ttu-id="b4c2f-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4c2f-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4c2f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4c2f-139">createdDateTime</span></span>|<span data-ttu-id="b4c2f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4c2f-140">DateTimeOffset</span></span>|<span data-ttu-id="b4c2f-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="b4c2f-141">DateTime the object was created.</span></span> <span data-ttu-id="b4c2f-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4c2f-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4c2f-143">description</span><span class="sxs-lookup"><span data-stu-id="b4c2f-143">description</span></span>|<span data-ttu-id="b4c2f-144">String</span><span class="sxs-lookup"><span data-stu-id="b4c2f-144">String</span></span>|<span data-ttu-id="b4c2f-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b4c2f-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b4c2f-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4c2f-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4c2f-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b4c2f-147">displayName</span></span>|<span data-ttu-id="b4c2f-148">String</span><span class="sxs-lookup"><span data-stu-id="b4c2f-148">String</span></span>|<span data-ttu-id="b4c2f-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="b4c2f-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b4c2f-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4c2f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b4c2f-151">Version</span><span class="sxs-lookup"><span data-stu-id="b4c2f-151">version</span></span>|<span data-ttu-id="b4c2f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b4c2f-152">Int32</span></span>|<span data-ttu-id="b4c2f-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="b4c2f-153">Version of the device configuration.</span></span> <span data-ttu-id="b4c2f-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4c2f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="b4c2f-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4c2f-155">Response</span></span>
<span data-ttu-id="b4c2f-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b4c2f-156">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4c2f-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4c2f-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="b4c2f-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4c2f-158">Request</span></span>
<span data-ttu-id="b4c2f-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4c2f-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="b4c2f-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4c2f-160">Response</span></span>
<span data-ttu-id="b4c2f-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4c2f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 342

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```


