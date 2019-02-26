---
title: Erstellen von „macOSDeviceFeaturesConfiguration“
description: Diese Methode erstellt ein neues Objekt des Typs macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e05ad426fc3457de535ff5db4718b52a30bb66e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252791"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="e578a-103">Erstellen von „macOSDeviceFeaturesConfiguration“</span><span class="sxs-lookup"><span data-stu-id="e578a-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="e578a-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e578a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e578a-105">Diese Methode erstellt ein neues Objekt des Typs [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e578a-105">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e578a-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e578a-106">Prerequisites</span></span>
<span data-ttu-id="e578a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e578a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e578a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e578a-109">Permission type</span></span>|<span data-ttu-id="e578a-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e578a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e578a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e578a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e578a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e578a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e578a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e578a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e578a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e578a-114">Not supported.</span></span>|
|<span data-ttu-id="e578a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e578a-115">Application</span></span>|<span data-ttu-id="e578a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e578a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e578a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e578a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e578a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e578a-118">Request headers</span></span>
|<span data-ttu-id="e578a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e578a-119">Header</span></span>|<span data-ttu-id="e578a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e578a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e578a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e578a-121">Authorization</span></span>|<span data-ttu-id="e578a-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e578a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e578a-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e578a-123">Accept</span></span>|<span data-ttu-id="e578a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e578a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e578a-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e578a-125">Request body</span></span>
<span data-ttu-id="e578a-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „macOSDeviceFeaturesConfiguration“ an.</span><span class="sxs-lookup"><span data-stu-id="e578a-126">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="e578a-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „macOSDeviceFeaturesConfiguration“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="e578a-127">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="e578a-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e578a-128">Property</span></span>|<span data-ttu-id="e578a-129">Typ</span><span class="sxs-lookup"><span data-stu-id="e578a-129">Type</span></span>|<span data-ttu-id="e578a-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e578a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e578a-131">id</span><span class="sxs-lookup"><span data-stu-id="e578a-131">id</span></span>|<span data-ttu-id="e578a-132">string</span><span class="sxs-lookup"><span data-stu-id="e578a-132">String</span></span>|<span data-ttu-id="e578a-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e578a-133">Key of the entity.</span></span> <span data-ttu-id="e578a-134">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e578a-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e578a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e578a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e578a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e578a-136">DateTimeOffset</span></span>|<span data-ttu-id="e578a-137">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e578a-137">DateTime the object was last modified.</span></span> <span data-ttu-id="e578a-138">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e578a-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e578a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e578a-139">createdDateTime</span></span>|<span data-ttu-id="e578a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e578a-140">DateTimeOffset</span></span>|<span data-ttu-id="e578a-141">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e578a-141">DateTime the object was created.</span></span> <span data-ttu-id="e578a-142">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e578a-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e578a-143">description</span><span class="sxs-lookup"><span data-stu-id="e578a-143">description</span></span>|<span data-ttu-id="e578a-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e578a-144">String</span></span>|<span data-ttu-id="e578a-145">Beschreibung der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e578a-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e578a-146">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e578a-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e578a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e578a-147">displayName</span></span>|<span data-ttu-id="e578a-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e578a-148">String</span></span>|<span data-ttu-id="e578a-149">Name der Gerätekonfiguration (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="e578a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e578a-150">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e578a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e578a-151">Version</span><span class="sxs-lookup"><span data-stu-id="e578a-151">version</span></span>|<span data-ttu-id="e578a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e578a-152">Int32</span></span>|<span data-ttu-id="e578a-153">Version der Gerätekonfiguration.</span><span class="sxs-lookup"><span data-stu-id="e578a-153">Version of the device configuration.</span></span> <span data-ttu-id="e578a-154">Geerbt von [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e578a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e578a-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="e578a-155">Response</span></span>
<span data-ttu-id="e578a-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e578a-156">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e578a-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e578a-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="e578a-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e578a-158">Request</span></span>
<span data-ttu-id="e578a-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e578a-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e578a-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="e578a-160">Response</span></span>
<span data-ttu-id="e578a-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e578a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



