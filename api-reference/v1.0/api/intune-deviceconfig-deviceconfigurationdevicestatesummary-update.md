---
title: Aktualisieren von „deviceConfigurationDeviceStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceStateSummary.
ms.openlocfilehash: a65ce289ad7c5c95b9a5ba344493c46d3dd14822
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018710"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="3213f-103">Aktualisieren von „deviceConfigurationDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="3213f-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="3213f-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3213f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3213f-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3213f-105">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3213f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3213f-106">Prerequisites</span></span>
<span data-ttu-id="3213f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3213f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3213f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3213f-109">Permission type</span></span>|<span data-ttu-id="3213f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3213f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3213f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3213f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3213f-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3213f-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3213f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3213f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3213f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3213f-114">Not supported.</span></span>|
|<span data-ttu-id="3213f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3213f-115">Application</span></span>|<span data-ttu-id="3213f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3213f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3213f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3213f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="3213f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3213f-118">Request headers</span></span>
|<span data-ttu-id="3213f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3213f-119">Header</span></span>|<span data-ttu-id="3213f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3213f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3213f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3213f-121">Authorization</span></span>|<span data-ttu-id="3213f-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3213f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3213f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3213f-123">Accept</span></span>|<span data-ttu-id="3213f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3213f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3213f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3213f-125">Request body</span></span>
<span data-ttu-id="3213f-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="3213f-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="3213f-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="3213f-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="3213f-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3213f-128">Property</span></span>|<span data-ttu-id="3213f-129">Typ</span><span class="sxs-lookup"><span data-stu-id="3213f-129">Type</span></span>|<span data-ttu-id="3213f-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3213f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3213f-131">id</span><span class="sxs-lookup"><span data-stu-id="3213f-131">id</span></span>|<span data-ttu-id="3213f-132">String</span><span class="sxs-lookup"><span data-stu-id="3213f-132">String</span></span>|<span data-ttu-id="3213f-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3213f-133">Key of the entity.</span></span>|
|<span data-ttu-id="3213f-134">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3213f-134">unknownDeviceCount</span></span>|<span data-ttu-id="3213f-135">Int32</span><span class="sxs-lookup"><span data-stu-id="3213f-135">Int32</span></span>|<span data-ttu-id="3213f-136">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="3213f-136">Number of unknown devices</span></span>|
|<span data-ttu-id="3213f-137">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3213f-137">notApplicableDeviceCount</span></span>|<span data-ttu-id="3213f-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3213f-138">Int32</span></span>|<span data-ttu-id="3213f-139">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="3213f-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="3213f-140">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3213f-140">compliantDeviceCount</span></span>|<span data-ttu-id="3213f-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3213f-141">Int32</span></span>|<span data-ttu-id="3213f-142">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="3213f-142">Number of compliant devices</span></span>|
|<span data-ttu-id="3213f-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3213f-143">remediatedDeviceCount</span></span>|<span data-ttu-id="3213f-144">Int32</span><span class="sxs-lookup"><span data-stu-id="3213f-144">Int32</span></span>|<span data-ttu-id="3213f-145">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="3213f-145">Number of remediated devices</span></span>|
|<span data-ttu-id="3213f-146">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3213f-146">nonCompliantDeviceCount</span></span>|<span data-ttu-id="3213f-147">Int32</span><span class="sxs-lookup"><span data-stu-id="3213f-147">Int32</span></span>|<span data-ttu-id="3213f-148">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="3213f-148">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="3213f-149">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3213f-149">errorDeviceCount</span></span>|<span data-ttu-id="3213f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3213f-150">Int32</span></span>|<span data-ttu-id="3213f-151">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="3213f-151">Number of error devices</span></span>|
|<span data-ttu-id="3213f-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3213f-152">conflictDeviceCount</span></span>|<span data-ttu-id="3213f-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3213f-153">Int32</span></span>|<span data-ttu-id="3213f-154">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="3213f-154">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="3213f-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="3213f-155">Response</span></span>
<span data-ttu-id="3213f-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3213f-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3213f-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3213f-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="3213f-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3213f-158">Request</span></span>
<span data-ttu-id="3213f-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3213f-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="3213f-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="3213f-160">Response</span></span>
<span data-ttu-id="3213f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3213f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```


