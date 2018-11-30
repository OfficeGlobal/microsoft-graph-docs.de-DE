---
title: Erstellen von „detectedApp“
description: Diese Methode erstellt ein neues Objekt des Typs detectedApp.
ms.openlocfilehash: c0875d2872ff40a1b19654b5aeb4dfc48483114e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018711"
---
# <a name="create-detectedapp"></a><span data-ttu-id="3540b-103">Erstellen von „detectedApp“</span><span class="sxs-lookup"><span data-stu-id="3540b-103">Create detectedApp</span></span>

> <span data-ttu-id="3540b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3540b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3540b-105">Diese Methode erstellt ein neues Objekt des Typs [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="3540b-105">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3540b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3540b-106">Prerequisites</span></span>
<span data-ttu-id="3540b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3540b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3540b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3540b-109">Permission type</span></span>|<span data-ttu-id="3540b-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3540b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3540b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3540b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3540b-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3540b-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3540b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3540b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3540b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3540b-114">Not supported.</span></span>|
|<span data-ttu-id="3540b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3540b-115">Application</span></span>|<span data-ttu-id="3540b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3540b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3540b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3540b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="3540b-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3540b-118">Request headers</span></span>
|<span data-ttu-id="3540b-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3540b-119">Header</span></span>|<span data-ttu-id="3540b-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3540b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3540b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3540b-121">Authorization</span></span>|<span data-ttu-id="3540b-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3540b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3540b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3540b-123">Accept</span></span>|<span data-ttu-id="3540b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3540b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3540b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3540b-125">Request body</span></span>
<span data-ttu-id="3540b-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „detectedApp“ an.</span><span class="sxs-lookup"><span data-stu-id="3540b-126">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="3540b-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „detectedApp“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="3540b-127">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="3540b-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3540b-128">Property</span></span>|<span data-ttu-id="3540b-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3540b-129">Type</span></span>|<span data-ttu-id="3540b-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3540b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3540b-131">id</span><span class="sxs-lookup"><span data-stu-id="3540b-131">id</span></span>|<span data-ttu-id="3540b-132">String</span><span class="sxs-lookup"><span data-stu-id="3540b-132">String</span></span>|<span data-ttu-id="3540b-133">Eindeutiger Bezeichner für die erkannte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="3540b-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="3540b-134">Dieser wird automatisch von Intune generiert, wenn die Anwendung erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="3540b-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="3540b-135">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3540b-135">Read-only.</span></span>|
|<span data-ttu-id="3540b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3540b-136">displayName</span></span>|<span data-ttu-id="3540b-137">String</span><span class="sxs-lookup"><span data-stu-id="3540b-137">String</span></span>|<span data-ttu-id="3540b-138">Name der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="3540b-138">Name of the discovered application.</span></span> <span data-ttu-id="3540b-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3540b-139">Read-only</span></span>|
|<span data-ttu-id="3540b-140">version</span><span class="sxs-lookup"><span data-stu-id="3540b-140">version</span></span>|<span data-ttu-id="3540b-141">String</span><span class="sxs-lookup"><span data-stu-id="3540b-141">String</span></span>|<span data-ttu-id="3540b-142">Version der ermittelten Anwendung.</span><span class="sxs-lookup"><span data-stu-id="3540b-142">Version of the discovered application.</span></span> <span data-ttu-id="3540b-143">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3540b-143">Read-only</span></span>|
|<span data-ttu-id="3540b-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="3540b-144">sizeInByte</span></span>|<span data-ttu-id="3540b-145">Int64</span><span class="sxs-lookup"><span data-stu-id="3540b-145">Int64</span></span>|<span data-ttu-id="3540b-146">Größe der ermittelten Anwendung in Byte.</span><span class="sxs-lookup"><span data-stu-id="3540b-146">Discovered application size in bytes.</span></span> <span data-ttu-id="3540b-147">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="3540b-147">Read-only</span></span>|
|<span data-ttu-id="3540b-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="3540b-148">deviceCount</span></span>|<span data-ttu-id="3540b-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3540b-149">Int32</span></span>|<span data-ttu-id="3540b-150">Anzahl von Geräten, auf denen die Anwendung installiert ist</span><span class="sxs-lookup"><span data-stu-id="3540b-150">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="3540b-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="3540b-151">Response</span></span>
<span data-ttu-id="3540b-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [detectedApp](../resources/intune-devices-detectedapp.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3540b-152">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3540b-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3540b-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="3540b-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3540b-154">Request</span></span>
<span data-ttu-id="3540b-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3540b-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
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

### <a name="response"></a><span data-ttu-id="3540b-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="3540b-156">Response</span></span>
<span data-ttu-id="3540b-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3540b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



