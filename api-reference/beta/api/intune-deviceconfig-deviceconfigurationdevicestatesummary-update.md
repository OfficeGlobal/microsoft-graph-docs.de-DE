---
title: Aktualisieren von „deviceConfigurationDeviceStateSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationDeviceStateSummary.
ms.openlocfilehash: 877fb15d8420933b2a9b87ae0723dd0335a9ff0d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065401"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="8e8af-103">Aktualisieren von „deviceConfigurationDeviceStateSummary“</span><span class="sxs-lookup"><span data-stu-id="8e8af-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="8e8af-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8e8af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e8af-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8e8af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e8af-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8e8af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e8af-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="8e8af-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e8af-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="8e8af-108">Prerequisites</span></span>
<span data-ttu-id="8e8af-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e8af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e8af-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8e8af-111">Permission type</span></span>|<span data-ttu-id="8e8af-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8e8af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e8af-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8e8af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e8af-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e8af-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e8af-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8e8af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e8af-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e8af-116">Not supported.</span></span>|
|<span data-ttu-id="8e8af-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8e8af-117">Application</span></span>|<span data-ttu-id="8e8af-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8e8af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e8af-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e8af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="8e8af-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8e8af-120">Request headers</span></span>
|<span data-ttu-id="8e8af-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8e8af-121">Header</span></span>|<span data-ttu-id="8e8af-122">Wert</span><span class="sxs-lookup"><span data-stu-id="8e8af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e8af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e8af-123">Authorization</span></span>|<span data-ttu-id="8e8af-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="8e8af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e8af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8e8af-125">Accept</span></span>|<span data-ttu-id="8e8af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e8af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e8af-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8e8af-127">Request body</span></span>
<span data-ttu-id="8e8af-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="8e8af-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="8e8af-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="8e8af-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="8e8af-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8e8af-130">Property</span></span>|<span data-ttu-id="8e8af-131">Typ</span><span class="sxs-lookup"><span data-stu-id="8e8af-131">Type</span></span>|<span data-ttu-id="8e8af-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8e8af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e8af-133">id</span><span class="sxs-lookup"><span data-stu-id="8e8af-133">id</span></span>|<span data-ttu-id="8e8af-134">String</span><span class="sxs-lookup"><span data-stu-id="8e8af-134">String</span></span>|<span data-ttu-id="8e8af-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="8e8af-135">Key of the entity.</span></span>|
|<span data-ttu-id="8e8af-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e8af-136">unknownDeviceCount</span></span>|<span data-ttu-id="8e8af-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8e8af-137">Int32</span></span>|<span data-ttu-id="8e8af-138">Anzahl von unbekannten Geräten</span><span class="sxs-lookup"><span data-stu-id="8e8af-138">Number of unknown devices</span></span>|
|<span data-ttu-id="8e8af-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e8af-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="8e8af-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8e8af-140">Int32</span></span>|<span data-ttu-id="8e8af-141">Anzahl der ausgenommenen Geräte</span><span class="sxs-lookup"><span data-stu-id="8e8af-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="8e8af-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e8af-142">compliantDeviceCount</span></span>|<span data-ttu-id="8e8af-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8e8af-143">Int32</span></span>|<span data-ttu-id="8e8af-144">Anzahl von konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="8e8af-144">Number of compliant devices</span></span>|
|<span data-ttu-id="8e8af-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e8af-145">remediatedDeviceCount</span></span>|<span data-ttu-id="8e8af-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8e8af-146">Int32</span></span>|<span data-ttu-id="8e8af-147">Anzahl von korrigierten Geräten</span><span class="sxs-lookup"><span data-stu-id="8e8af-147">Number of remediated devices</span></span>|
|<span data-ttu-id="8e8af-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e8af-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="8e8af-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8e8af-149">Int32</span></span>|<span data-ttu-id="8e8af-150">Anzahl von nicht konformen Geräten</span><span class="sxs-lookup"><span data-stu-id="8e8af-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="8e8af-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e8af-151">errorDeviceCount</span></span>|<span data-ttu-id="8e8af-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8e8af-152">Int32</span></span>|<span data-ttu-id="8e8af-153">Anzahl von Geräten mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="8e8af-153">Number of error devices</span></span>|
|<span data-ttu-id="8e8af-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8e8af-154">conflictDeviceCount</span></span>|<span data-ttu-id="8e8af-155">Int32</span><span class="sxs-lookup"><span data-stu-id="8e8af-155">Int32</span></span>|<span data-ttu-id="8e8af-156">Anzahl von Geräten mit Konflikt</span><span class="sxs-lookup"><span data-stu-id="8e8af-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="8e8af-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e8af-157">Response</span></span>
<span data-ttu-id="8e8af-158">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8e8af-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e8af-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8e8af-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e8af-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8e8af-160">Request</span></span>
<span data-ttu-id="8e8af-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8e8af-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 214

{
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="8e8af-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="8e8af-162">Response</span></span>
<span data-ttu-id="8e8af-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8e8af-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





