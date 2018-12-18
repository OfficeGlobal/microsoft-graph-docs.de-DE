---
title: Aktualisieren von „managedDeviceMobileAppConfigurationUserSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceMobileAppConfigurationUserSummary.
author: tfitzmac
ms.openlocfilehash: b5b639bf517867ca23634c9af788ccbf91396b67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333908"
---
# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="b48fe-103">Aktualisieren von „managedDeviceMobileAppConfigurationUserSummary“</span><span class="sxs-lookup"><span data-stu-id="b48fe-103">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="b48fe-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b48fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b48fe-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b48fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b48fe-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b48fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b48fe-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span><span class="sxs-lookup"><span data-stu-id="b48fe-107">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b48fe-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b48fe-108">Prerequisites</span></span>
<span data-ttu-id="b48fe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b48fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b48fe-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b48fe-111">Permission type</span></span>|<span data-ttu-id="b48fe-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b48fe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b48fe-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b48fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b48fe-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b48fe-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b48fe-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b48fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b48fe-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b48fe-116">Not supported.</span></span>|
|<span data-ttu-id="b48fe-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b48fe-117">Application</span></span>|<span data-ttu-id="b48fe-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b48fe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b48fe-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b48fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="b48fe-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b48fe-120">Request headers</span></span>
|<span data-ttu-id="b48fe-121">Header</span><span class="sxs-lookup"><span data-stu-id="b48fe-121">Header</span></span>|<span data-ttu-id="b48fe-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b48fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b48fe-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b48fe-123">Authorization</span></span>|<span data-ttu-id="b48fe-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b48fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b48fe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b48fe-125">Accept</span></span>|<span data-ttu-id="b48fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b48fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b48fe-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b48fe-127">Request body</span></span>
<span data-ttu-id="b48fe-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="b48fe-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="b48fe-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="b48fe-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="b48fe-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b48fe-130">Property</span></span>|<span data-ttu-id="b48fe-131">Typ</span><span class="sxs-lookup"><span data-stu-id="b48fe-131">Type</span></span>|<span data-ttu-id="b48fe-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b48fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b48fe-133">id</span><span class="sxs-lookup"><span data-stu-id="b48fe-133">id</span></span>|<span data-ttu-id="b48fe-134">String</span><span class="sxs-lookup"><span data-stu-id="b48fe-134">String</span></span>|<span data-ttu-id="b48fe-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b48fe-135">Key of the entity.</span></span>|
|<span data-ttu-id="b48fe-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="b48fe-136">pendingCount</span></span>|<span data-ttu-id="b48fe-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b48fe-137">Int32</span></span>|<span data-ttu-id="b48fe-138">Anzahl der ausstehenden Benutzer</span><span class="sxs-lookup"><span data-stu-id="b48fe-138">Number of pending Users</span></span>|
|<span data-ttu-id="b48fe-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="b48fe-139">notApplicableCount</span></span>|<span data-ttu-id="b48fe-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b48fe-140">Int32</span></span>|<span data-ttu-id="b48fe-141">Anzahl der Benutzer nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="b48fe-141">Number of not applicable users</span></span>|
|<span data-ttu-id="b48fe-142">successCount</span><span class="sxs-lookup"><span data-stu-id="b48fe-142">successCount</span></span>|<span data-ttu-id="b48fe-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b48fe-143">Int32</span></span>|<span data-ttu-id="b48fe-144">Anzahl der erfolgreichen Benutzer</span><span class="sxs-lookup"><span data-stu-id="b48fe-144">Number of succeeded Users</span></span>|
|<span data-ttu-id="b48fe-145">errorCount</span><span class="sxs-lookup"><span data-stu-id="b48fe-145">errorCount</span></span>|<span data-ttu-id="b48fe-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b48fe-146">Int32</span></span>|<span data-ttu-id="b48fe-147">Anzahl der Benutzer mit Fehlern</span><span class="sxs-lookup"><span data-stu-id="b48fe-147">Number of error Users</span></span>|
|<span data-ttu-id="b48fe-148">failedCount</span><span class="sxs-lookup"><span data-stu-id="b48fe-148">failedCount</span></span>|<span data-ttu-id="b48fe-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b48fe-149">Int32</span></span>|<span data-ttu-id="b48fe-150">Anzahl der fehlgeschlagenen Benutzer</span><span class="sxs-lookup"><span data-stu-id="b48fe-150">Number of failed Users</span></span>|
|<span data-ttu-id="b48fe-151">conflictCount</span><span class="sxs-lookup"><span data-stu-id="b48fe-151">conflictCount</span></span>|<span data-ttu-id="b48fe-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b48fe-152">Int32</span></span>|<span data-ttu-id="b48fe-153">Anzahl von Benutzern in Konflikt</span><span class="sxs-lookup"><span data-stu-id="b48fe-153">Number of users in conflict</span></span>|
|<span data-ttu-id="b48fe-154">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b48fe-154">lastUpdateDateTime</span></span>|<span data-ttu-id="b48fe-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b48fe-155">DateTimeOffset</span></span>|<span data-ttu-id="b48fe-156">Datum und Uhrzeit der letzten Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="b48fe-156">Last update time</span></span>|
|<span data-ttu-id="b48fe-157">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="b48fe-157">configurationVersion</span></span>|<span data-ttu-id="b48fe-158">Int32</span><span class="sxs-lookup"><span data-stu-id="b48fe-158">Int32</span></span>|<span data-ttu-id="b48fe-159">Version der Richtlinie für diese Übersicht</span><span class="sxs-lookup"><span data-stu-id="b48fe-159">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="b48fe-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="b48fe-160">Response</span></span>
<span data-ttu-id="b48fe-161">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) zurück.</span><span class="sxs-lookup"><span data-stu-id="b48fe-161">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b48fe-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b48fe-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="b48fe-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b48fe-163">Request</span></span>
<span data-ttu-id="b48fe-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b48fe-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
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

### <a name="response"></a><span data-ttu-id="b48fe-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="b48fe-165">Response</span></span>
<span data-ttu-id="b48fe-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b48fe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 370

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
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





