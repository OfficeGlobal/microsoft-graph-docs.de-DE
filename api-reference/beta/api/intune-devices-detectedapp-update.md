---
title: Aktualisieren von „detectedApp“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs detectedApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 550bbcfd422f12bc3c11102e3438ffab0162680b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862951"
---
# <a name="update-detectedapp"></a><span data-ttu-id="647af-103">Aktualisieren von „detectedApp“</span><span class="sxs-lookup"><span data-stu-id="647af-103">Update detectedApp</span></span>

> <span data-ttu-id="647af-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="647af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="647af-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="647af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="647af-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="647af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="647af-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="647af-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="647af-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="647af-108">Prerequisites</span></span>
<span data-ttu-id="647af-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="647af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="647af-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="647af-111">Permission type</span></span>|<span data-ttu-id="647af-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="647af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="647af-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="647af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="647af-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="647af-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="647af-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="647af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="647af-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="647af-116">Not supported.</span></span>|
|<span data-ttu-id="647af-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="647af-117">Application</span></span>|<span data-ttu-id="647af-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="647af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="647af-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="647af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="647af-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="647af-120">Request headers</span></span>
|<span data-ttu-id="647af-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="647af-121">Header</span></span>|<span data-ttu-id="647af-122">Wert</span><span class="sxs-lookup"><span data-stu-id="647af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="647af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="647af-123">Authorization</span></span>|<span data-ttu-id="647af-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="647af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="647af-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="647af-125">Accept</span></span>|<span data-ttu-id="647af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="647af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="647af-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="647af-127">Request body</span></span>
<span data-ttu-id="647af-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [detectedApp](../resources/intune-devices-detectedapp.md) an.</span><span class="sxs-lookup"><span data-stu-id="647af-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="647af-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [detectedApp](../resources/intune-devices-detectedapp.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="647af-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="647af-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="647af-130">Property</span></span>|<span data-ttu-id="647af-131">Typ</span><span class="sxs-lookup"><span data-stu-id="647af-131">Type</span></span>|<span data-ttu-id="647af-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="647af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="647af-133">id</span><span class="sxs-lookup"><span data-stu-id="647af-133">id</span></span>|<span data-ttu-id="647af-134">String</span><span class="sxs-lookup"><span data-stu-id="647af-134">String</span></span>|<span data-ttu-id="647af-135">Eindeutiger Bezeichner für die erkannte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="647af-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="647af-136">Dieser wird automatisch von Intune generiert, wenn die Anwendung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="647af-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="647af-137">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="647af-137">Read-only.</span></span>|
|<span data-ttu-id="647af-138">displayName</span><span class="sxs-lookup"><span data-stu-id="647af-138">displayName</span></span>|<span data-ttu-id="647af-139">String</span><span class="sxs-lookup"><span data-stu-id="647af-139">String</span></span>|<span data-ttu-id="647af-140">Name der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="647af-140">Name of the discovered application.</span></span> <span data-ttu-id="647af-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="647af-141">Read-only</span></span>|
|<span data-ttu-id="647af-142">version</span><span class="sxs-lookup"><span data-stu-id="647af-142">version</span></span>|<span data-ttu-id="647af-143">String</span><span class="sxs-lookup"><span data-stu-id="647af-143">String</span></span>|<span data-ttu-id="647af-144">Version der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="647af-144">Version of the discovered application.</span></span> <span data-ttu-id="647af-145">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="647af-145">Read-only</span></span>|
|<span data-ttu-id="647af-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="647af-146">sizeInByte</span></span>|<span data-ttu-id="647af-147">Int64</span><span class="sxs-lookup"><span data-stu-id="647af-147">Int64</span></span>|<span data-ttu-id="647af-148">Größe der ermittelten Anwendung in Byte.</span><span class="sxs-lookup"><span data-stu-id="647af-148">Discovered application size in bytes.</span></span> <span data-ttu-id="647af-149">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="647af-149">Read-only</span></span>|
|<span data-ttu-id="647af-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="647af-150">deviceCount</span></span>|<span data-ttu-id="647af-151">Int32</span><span class="sxs-lookup"><span data-stu-id="647af-151">Int32</span></span>|<span data-ttu-id="647af-152">Anzahl von Geräten, auf denen die Anwendung installiert ist</span><span class="sxs-lookup"><span data-stu-id="647af-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="647af-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="647af-153">Response</span></span>
<span data-ttu-id="647af-154">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [detectedApp](../resources/intune-devices-detectedapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="647af-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="647af-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="647af-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="647af-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="647af-156">Request</span></span>
<span data-ttu-id="647af-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="647af-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
Content-type: application/json
Content-length: 117

{
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="647af-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="647af-158">Response</span></span>
<span data-ttu-id="647af-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="647af-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





