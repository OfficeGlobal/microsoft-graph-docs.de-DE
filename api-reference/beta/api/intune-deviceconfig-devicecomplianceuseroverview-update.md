---
title: Aktualisieren von „deviceComplianceUserOverview“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceComplianceUserOverview.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 05ccf80b957bf52155dfef738c886cf41155fc22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891105"
---
# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="69b4a-103">Aktualisieren von „deviceComplianceUserOverview“</span><span class="sxs-lookup"><span data-stu-id="69b4a-103">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="69b4a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="69b4a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69b4a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="69b4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69b4a-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="69b4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69b4a-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span><span class="sxs-lookup"><span data-stu-id="69b4a-107">Update the properties of a [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69b4a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="69b4a-108">Prerequisites</span></span>
<span data-ttu-id="69b4a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69b4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69b4a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="69b4a-111">Permission type</span></span>|<span data-ttu-id="69b4a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="69b4a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69b4a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="69b4a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="69b4a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69b4a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="69b4a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="69b4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69b4a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69b4a-116">Not supported.</span></span>|
|<span data-ttu-id="69b4a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="69b4a-117">Application</span></span>|<span data-ttu-id="69b4a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69b4a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69b4a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="69b4a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="69b4a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="69b4a-120">Request headers</span></span>
|<span data-ttu-id="69b4a-121">Header</span><span class="sxs-lookup"><span data-stu-id="69b4a-121">Header</span></span>|<span data-ttu-id="69b4a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="69b4a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69b4a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69b4a-123">Authorization</span></span>|<span data-ttu-id="69b4a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="69b4a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69b4a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="69b4a-125">Accept</span></span>|<span data-ttu-id="69b4a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="69b4a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69b4a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="69b4a-127">Request body</span></span>
<span data-ttu-id="69b4a-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) an.</span><span class="sxs-lookup"><span data-stu-id="69b4a-128">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="69b4a-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="69b4a-129">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="69b4a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="69b4a-130">Property</span></span>|<span data-ttu-id="69b4a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="69b4a-131">Type</span></span>|<span data-ttu-id="69b4a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69b4a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69b4a-133">id</span><span class="sxs-lookup"><span data-stu-id="69b4a-133">id</span></span>|<span data-ttu-id="69b4a-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="69b4a-134">String</span></span>|<span data-ttu-id="69b4a-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="69b4a-135">Key of the entity.</span></span>|
|<span data-ttu-id="69b4a-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="69b4a-136">pendingCount</span></span>|<span data-ttu-id="69b4a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="69b4a-137">Int32</span></span>|<span data-ttu-id="69b4a-138">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="69b4a-138">Number of pending Users</span></span>|
|<span data-ttu-id="69b4a-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="69b4a-139">notApplicableCount</span></span>|<span data-ttu-id="69b4a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="69b4a-140">Int32</span></span>|<span data-ttu-id="69b4a-141">Anzahl der Benutzer nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="69b4a-141">Number of not applicable users</span></span>|
|<span data-ttu-id="69b4a-142">successCount</span><span class="sxs-lookup"><span data-stu-id="69b4a-142">successCount</span></span>|<span data-ttu-id="69b4a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="69b4a-143">Int32</span></span>|<span data-ttu-id="69b4a-144">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="69b4a-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="69b4a-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="69b4a-145">errorCount</span></span>|<span data-ttu-id="69b4a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="69b4a-146">Int32</span></span>|<span data-ttu-id="69b4a-147">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="69b4a-147">Number of error Users</span></span>|
|<span data-ttu-id="69b4a-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="69b4a-148">failedCount</span></span>|<span data-ttu-id="69b4a-149">Int32</span><span class="sxs-lookup"><span data-stu-id="69b4a-149">Int32</span></span>|<span data-ttu-id="69b4a-150">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="69b4a-150">Number of failed Users</span></span>|
|<span data-ttu-id="69b4a-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="69b4a-151">conflictCount</span></span>|<span data-ttu-id="69b4a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="69b4a-152">Int32</span></span>|<span data-ttu-id="69b4a-153">Anzahl von Benutzern in Konflikt</span><span class="sxs-lookup"><span data-stu-id="69b4a-153">Number of users in conflict</span></span>|
|<span data-ttu-id="69b4a-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="69b4a-154">lastUpdateDateTime</span></span>|<span data-ttu-id="69b4a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69b4a-155">DateTimeOffset</span></span>|<span data-ttu-id="69b4a-156">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="69b4a-156">Last update time</span></span>|
|<span data-ttu-id="69b4a-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="69b4a-157">configurationVersion</span></span>|<span data-ttu-id="69b4a-158">Int32</span><span class="sxs-lookup"><span data-stu-id="69b4a-158">Int32</span></span>|<span data-ttu-id="69b4a-159">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="69b4a-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="69b4a-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="69b4a-160">Response</span></span>
<span data-ttu-id="69b4a-161">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="69b4a-161">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune-deviceconfig-devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69b4a-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="69b4a-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="69b4a-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="69b4a-163">Request</span></span>
<span data-ttu-id="69b4a-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="69b4a-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
Content-type: application/json
Content-length: 236

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="69b4a-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="69b4a-165">Response</span></span>
<span data-ttu-id="69b4a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69b4a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 352

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```





