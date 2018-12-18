---
title: Aktualisieren von „managedDeviceMobileAppConfigurationUserSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceMobileAppConfigurationUserSummary.
author: tfitzmac
ms.openlocfilehash: 35bcbfd5970b263b6fc0b76b0624361466dbbd68
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359465"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="caaec-103">Aktualisieren von „managedDeviceMobileAppConfigurationUserSummary“</span><span class="sxs-lookup"><span data-stu-id="caaec-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="caaec-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="caaec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="caaec-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="caaec-105">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="caaec-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="caaec-106">Prerequisites</span></span>
<span data-ttu-id="caaec-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="caaec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="caaec-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="caaec-109">Permission type</span></span>|<span data-ttu-id="caaec-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="caaec-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="caaec-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="caaec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="caaec-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caaec-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="caaec-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="caaec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="caaec-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="caaec-114">Not supported.</span></span>|
|<span data-ttu-id="caaec-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="caaec-115">Application</span></span>|<span data-ttu-id="caaec-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="caaec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="caaec-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="caaec-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="caaec-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="caaec-118">Request headers</span></span>
|<span data-ttu-id="caaec-119">Header</span><span class="sxs-lookup"><span data-stu-id="caaec-119">Header</span></span>|<span data-ttu-id="caaec-120">Wert</span><span class="sxs-lookup"><span data-stu-id="caaec-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="caaec-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="caaec-121">Authorization</span></span>|<span data-ttu-id="caaec-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="caaec-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="caaec-123">Accept</span><span class="sxs-lookup"><span data-stu-id="caaec-123">Accept</span></span>|<span data-ttu-id="caaec-124">application/json</span><span class="sxs-lookup"><span data-stu-id="caaec-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="caaec-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="caaec-125">Request body</span></span>
<span data-ttu-id="caaec-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="caaec-126">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="caaec-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="caaec-127">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="caaec-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="caaec-128">Property</span></span>|<span data-ttu-id="caaec-129">Typ</span><span class="sxs-lookup"><span data-stu-id="caaec-129">Type</span></span>|<span data-ttu-id="caaec-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="caaec-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caaec-131">id</span><span class="sxs-lookup"><span data-stu-id="caaec-131">id</span></span>|<span data-ttu-id="caaec-132">String</span><span class="sxs-lookup"><span data-stu-id="caaec-132">String</span></span>|<span data-ttu-id="caaec-133">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="caaec-133">Key of the entity.</span></span>|
|<span data-ttu-id="caaec-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="caaec-134">pendingCount</span></span>|<span data-ttu-id="caaec-135">Int32</span><span class="sxs-lookup"><span data-stu-id="caaec-135">Int32</span></span>|<span data-ttu-id="caaec-136">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="caaec-136">Number of pending Users</span></span>|
|<span data-ttu-id="caaec-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="caaec-137">notApplicableCount</span></span>|<span data-ttu-id="caaec-138">Int32</span><span class="sxs-lookup"><span data-stu-id="caaec-138">Int32</span></span>|<span data-ttu-id="caaec-139">Anzahl der Benutzer nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="caaec-139">Number of not applicable users</span></span>|
|<span data-ttu-id="caaec-140">successCount</span><span class="sxs-lookup"><span data-stu-id="caaec-140">successCount</span></span>|<span data-ttu-id="caaec-141">Int32</span><span class="sxs-lookup"><span data-stu-id="caaec-141">Int32</span></span>|<span data-ttu-id="caaec-142">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="caaec-142">Number of succeeded Users</span></span>|
|<span data-ttu-id="caaec-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="caaec-143">errorCount</span></span>|<span data-ttu-id="caaec-144">Int32</span><span class="sxs-lookup"><span data-stu-id="caaec-144">Int32</span></span>|<span data-ttu-id="caaec-145">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="caaec-145">Number of error Users</span></span>|
|<span data-ttu-id="caaec-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="caaec-146">failedCount</span></span>|<span data-ttu-id="caaec-147">Int32</span><span class="sxs-lookup"><span data-stu-id="caaec-147">Int32</span></span>|<span data-ttu-id="caaec-148">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="caaec-148">Number of failed Users</span></span>|
|<span data-ttu-id="caaec-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="caaec-149">lastUpdateDateTime</span></span>|<span data-ttu-id="caaec-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="caaec-150">DateTimeOffset</span></span>|<span data-ttu-id="caaec-151">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="caaec-151">Last update time</span></span>|
|<span data-ttu-id="caaec-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="caaec-152">configurationVersion</span></span>|<span data-ttu-id="caaec-153">Int32</span><span class="sxs-lookup"><span data-stu-id="caaec-153">Int32</span></span>|<span data-ttu-id="caaec-154">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="caaec-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="caaec-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="caaec-155">Response</span></span>
<span data-ttu-id="caaec-156">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="caaec-156">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="caaec-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="caaec-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="caaec-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="caaec-158">Request</span></span>
<span data-ttu-id="caaec-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="caaec-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
Content-type: application/json
Content-length: 297

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="caaec-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="caaec-160">Response</span></span>
<span data-ttu-id="caaec-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="caaec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



