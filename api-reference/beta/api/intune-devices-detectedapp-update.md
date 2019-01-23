---
title: Aktualisieren von „detectedApp“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs detectedApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7bfea341aafb25ea010162d270eab451900c0d04
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394943"
---
# <a name="update-detectedapp"></a><span data-ttu-id="9f990-103">Aktualisieren von „detectedApp“</span><span class="sxs-lookup"><span data-stu-id="9f990-103">Update detectedApp</span></span>

> <span data-ttu-id="9f990-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9f990-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9f990-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f990-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f990-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f990-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f990-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9f990-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f990-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9f990-108">Prerequisites</span></span>
<span data-ttu-id="9f990-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f990-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9f990-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f990-111">Permission type</span></span>|<span data-ttu-id="9f990-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f990-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f990-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f990-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f990-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f990-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9f990-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f990-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f990-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f990-116">Not supported.</span></span>|
|<span data-ttu-id="9f990-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f990-117">Application</span></span>|<span data-ttu-id="9f990-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f990-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f990-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f990-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="9f990-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f990-120">Request headers</span></span>
|<span data-ttu-id="9f990-121">Header</span><span class="sxs-lookup"><span data-stu-id="9f990-121">Header</span></span>|<span data-ttu-id="9f990-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9f990-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f990-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9f990-123">Authorization</span></span>|<span data-ttu-id="9f990-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9f990-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f990-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9f990-125">Accept</span></span>|<span data-ttu-id="9f990-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f990-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f990-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f990-127">Request body</span></span>
<span data-ttu-id="9f990-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [detectedApp](../resources/intune-devices-detectedapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="9f990-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="9f990-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [detectedApp](../resources/intune-devices-detectedapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="9f990-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="9f990-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9f990-130">Property</span></span>|<span data-ttu-id="9f990-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9f990-131">Type</span></span>|<span data-ttu-id="9f990-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f990-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f990-133">id</span><span class="sxs-lookup"><span data-stu-id="9f990-133">id</span></span>|<span data-ttu-id="9f990-134">String</span><span class="sxs-lookup"><span data-stu-id="9f990-134">String</span></span>|<span data-ttu-id="9f990-135">Eindeutiger Bezeichner für die erkannte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="9f990-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="9f990-136">Dieser wird automatisch von Intune generiert, wenn die Anwendung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="9f990-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="9f990-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9f990-137">Read-only.</span></span>|
|<span data-ttu-id="9f990-138">displayName</span><span class="sxs-lookup"><span data-stu-id="9f990-138">displayName</span></span>|<span data-ttu-id="9f990-139">String</span><span class="sxs-lookup"><span data-stu-id="9f990-139">String</span></span>|<span data-ttu-id="9f990-140">Name der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="9f990-140">Name of the discovered application.</span></span> <span data-ttu-id="9f990-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9f990-141">Read-only</span></span>|
|<span data-ttu-id="9f990-142">version</span><span class="sxs-lookup"><span data-stu-id="9f990-142">version</span></span>|<span data-ttu-id="9f990-143">String</span><span class="sxs-lookup"><span data-stu-id="9f990-143">String</span></span>|<span data-ttu-id="9f990-144">Version der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="9f990-144">Version of the discovered application.</span></span> <span data-ttu-id="9f990-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9f990-145">Read-only</span></span>|
|<span data-ttu-id="9f990-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="9f990-146">sizeInByte</span></span>|<span data-ttu-id="9f990-147">Int64</span><span class="sxs-lookup"><span data-stu-id="9f990-147">Int64</span></span>|<span data-ttu-id="9f990-148">Größe der ermittelten Anwendung in Byte.</span><span class="sxs-lookup"><span data-stu-id="9f990-148">Discovered application size in bytes.</span></span> <span data-ttu-id="9f990-149">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="9f990-149">Read-only</span></span>|
|<span data-ttu-id="9f990-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="9f990-150">deviceCount</span></span>|<span data-ttu-id="9f990-151">Int32</span><span class="sxs-lookup"><span data-stu-id="9f990-151">Int32</span></span>|<span data-ttu-id="9f990-152">Anzahl von Geräten, auf denen die Anwendung installiert ist</span><span class="sxs-lookup"><span data-stu-id="9f990-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="9f990-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f990-153">Response</span></span>
<span data-ttu-id="9f990-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [detectedApp](../resources/intune-devices-detectedapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9f990-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f990-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f990-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f990-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f990-156">Request</span></span>
<span data-ttu-id="9f990-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f990-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f990-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f990-158">Response</span></span>
<span data-ttu-id="9f990-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f990-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




