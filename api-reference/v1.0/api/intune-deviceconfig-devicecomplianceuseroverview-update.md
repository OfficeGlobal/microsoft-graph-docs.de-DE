---
title: Aktualisieren von „deviceComplianceUserOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceUserOverview.
ms.openlocfilehash: 8bd9ad8c413d6414305cf8648eacee00cca32930
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018291"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="c155c-103">Aktualisieren von „deviceComplianceUserOverview“</span><span class="sxs-lookup"><span data-stu-id="c155c-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="c155c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c155c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c155c-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="c155c-105">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c155c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c155c-106">Prerequisites</span></span>
<span data-ttu-id="c155c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c155c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c155c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c155c-109">Permission type</span></span>|<span data-ttu-id="c155c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c155c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c155c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c155c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c155c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c155c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c155c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c155c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c155c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c155c-114">Not supported.</span></span>|
|<span data-ttu-id="c155c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c155c-115">Application</span></span>|<span data-ttu-id="c155c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c155c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c155c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c155c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="c155c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c155c-118">Request headers</span></span>
|<span data-ttu-id="c155c-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c155c-119">Header</span></span>|<span data-ttu-id="c155c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c155c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c155c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c155c-121">Authorization</span></span>|<span data-ttu-id="c155c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c155c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c155c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c155c-123">Accept</span></span>|<span data-ttu-id="c155c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c155c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c155c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c155c-125">Request body</span></span>
<span data-ttu-id="c155c-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="c155c-126">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="c155c-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="c155c-127">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="c155c-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c155c-128">Property</span></span>|<span data-ttu-id="c155c-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c155c-129">Type</span></span>|<span data-ttu-id="c155c-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c155c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c155c-131">id</span><span class="sxs-lookup"><span data-stu-id="c155c-131">id</span></span>|<span data-ttu-id="c155c-132">String</span><span class="sxs-lookup"><span data-stu-id="c155c-132">String</span></span>|<span data-ttu-id="c155c-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c155c-133">Key of the entity.</span></span>|
|<span data-ttu-id="c155c-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="c155c-134">pendingCount</span></span>|<span data-ttu-id="c155c-135">Int32</span><span class="sxs-lookup"><span data-stu-id="c155c-135">Int32</span></span>|<span data-ttu-id="c155c-136">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="c155c-136">Number of pending Users</span></span>|
|<span data-ttu-id="c155c-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c155c-137">notApplicableCount</span></span>|<span data-ttu-id="c155c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="c155c-138">Int32</span></span>|<span data-ttu-id="c155c-139">Anzahl der Benutzer nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="c155c-139">Number of not applicable users</span></span>|
|<span data-ttu-id="c155c-140">successCount</span><span class="sxs-lookup"><span data-stu-id="c155c-140">successCount</span></span>|<span data-ttu-id="c155c-141">Int32</span><span class="sxs-lookup"><span data-stu-id="c155c-141">Int32</span></span>|<span data-ttu-id="c155c-142">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="c155c-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="c155c-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="c155c-143">errorCount</span></span>|<span data-ttu-id="c155c-144">Int32</span><span class="sxs-lookup"><span data-stu-id="c155c-144">Int32</span></span>|<span data-ttu-id="c155c-145">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="c155c-145">Number of error Users</span></span>|
|<span data-ttu-id="c155c-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="c155c-146">failedCount</span></span>|<span data-ttu-id="c155c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="c155c-147">Int32</span></span>|<span data-ttu-id="c155c-148">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="c155c-148">Number of failed Users</span></span>|
|<span data-ttu-id="c155c-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="c155c-149">lastUpdateDateTime</span></span>|<span data-ttu-id="c155c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c155c-150">DateTimeOffset</span></span>|<span data-ttu-id="c155c-151">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="c155c-151">Last update time</span></span>|
|<span data-ttu-id="c155c-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="c155c-152">configurationVersion</span></span>|<span data-ttu-id="c155c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c155c-153">Int32</span></span>|<span data-ttu-id="c155c-154">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="c155c-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="c155c-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="c155c-155">Response</span></span>
<span data-ttu-id="c155c-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c155c-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c155c-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c155c-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="c155c-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c155c-158">Request</span></span>
<span data-ttu-id="c155c-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c155c-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="c155c-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="c155c-160">Response</span></span>
<span data-ttu-id="c155c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c155c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 328

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



