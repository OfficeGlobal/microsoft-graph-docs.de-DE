---
title: Aktualisieren von „detectedApp“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs detectedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a68a4d417d50015a4fa4dad406d494b9f21fc697
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170483"
---
# <a name="update-detectedapp"></a><span data-ttu-id="44491-103">Aktualisieren von „detectedApp“</span><span class="sxs-lookup"><span data-stu-id="44491-103">Update detectedApp</span></span>

> <span data-ttu-id="44491-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="44491-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44491-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="44491-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44491-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="44491-106">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44491-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="44491-107">Prerequisites</span></span>
<span data-ttu-id="44491-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="44491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="44491-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="44491-110">Permission type</span></span>|<span data-ttu-id="44491-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="44491-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44491-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="44491-112">Delegated (work or school account)</span></span>|<span data-ttu-id="44491-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44491-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="44491-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="44491-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44491-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44491-115">Not supported.</span></span>|
|<span data-ttu-id="44491-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="44491-116">Application</span></span>|<span data-ttu-id="44491-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="44491-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44491-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="44491-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="44491-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="44491-119">Request headers</span></span>
|<span data-ttu-id="44491-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="44491-120">Header</span></span>|<span data-ttu-id="44491-121">Wert</span><span class="sxs-lookup"><span data-stu-id="44491-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44491-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="44491-122">Authorization</span></span>|<span data-ttu-id="44491-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="44491-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44491-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="44491-124">Accept</span></span>|<span data-ttu-id="44491-125">application/json</span><span class="sxs-lookup"><span data-stu-id="44491-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44491-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="44491-126">Request body</span></span>
<span data-ttu-id="44491-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [detectedApp](../resources/intune-devices-detectedapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="44491-127">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="44491-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [detectedApp](../resources/intune-devices-detectedapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="44491-128">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="44491-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="44491-129">Property</span></span>|<span data-ttu-id="44491-130">Typ</span><span class="sxs-lookup"><span data-stu-id="44491-130">Type</span></span>|<span data-ttu-id="44491-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="44491-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44491-132">id</span><span class="sxs-lookup"><span data-stu-id="44491-132">id</span></span>|<span data-ttu-id="44491-133">string</span><span class="sxs-lookup"><span data-stu-id="44491-133">String</span></span>|<span data-ttu-id="44491-134">Eindeutiger Bezeichner für die erkannte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="44491-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="44491-135">Dieser wird automatisch von Intune generiert, wenn die Anwendung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="44491-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="44491-136">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="44491-136">Read-only.</span></span>|
|<span data-ttu-id="44491-137">displayName</span><span class="sxs-lookup"><span data-stu-id="44491-137">displayName</span></span>|<span data-ttu-id="44491-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="44491-138">String</span></span>|<span data-ttu-id="44491-139">Name der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="44491-139">Name of the discovered application.</span></span> <span data-ttu-id="44491-140">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="44491-140">Read-only</span></span>|
|<span data-ttu-id="44491-141">version</span><span class="sxs-lookup"><span data-stu-id="44491-141">version</span></span>|<span data-ttu-id="44491-142">String</span><span class="sxs-lookup"><span data-stu-id="44491-142">String</span></span>|<span data-ttu-id="44491-143">Version der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="44491-143">Version of the discovered application.</span></span> <span data-ttu-id="44491-144">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="44491-144">Read-only</span></span>|
|<span data-ttu-id="44491-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="44491-145">sizeInByte</span></span>|<span data-ttu-id="44491-146">Int64</span><span class="sxs-lookup"><span data-stu-id="44491-146">Int64</span></span>|<span data-ttu-id="44491-147">Größe der ermittelten Anwendung in Byte.</span><span class="sxs-lookup"><span data-stu-id="44491-147">Discovered application size in bytes.</span></span> <span data-ttu-id="44491-148">Schreibgeschützt</span><span class="sxs-lookup"><span data-stu-id="44491-148">Read-only</span></span>|
|<span data-ttu-id="44491-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="44491-149">deviceCount</span></span>|<span data-ttu-id="44491-150">Int32</span><span class="sxs-lookup"><span data-stu-id="44491-150">Int32</span></span>|<span data-ttu-id="44491-151">Anzahl von Geräten, auf denen die Anwendung installiert ist</span><span class="sxs-lookup"><span data-stu-id="44491-151">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="44491-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="44491-152">Response</span></span>
<span data-ttu-id="44491-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [detectedApp](../resources/intune-devices-detectedapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="44491-153">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44491-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="44491-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="44491-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="44491-155">Request</span></span>
<span data-ttu-id="44491-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="44491-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="44491-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="44491-157">Response</span></span>
<span data-ttu-id="44491-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="44491-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```




