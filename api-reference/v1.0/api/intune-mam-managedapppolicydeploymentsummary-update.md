---
title: Aktualisieren von „managedAppPolicyDeploymentSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedAppPolicyDeploymentSummary.
ms.openlocfilehash: 66f6e10dda834eca3ffa728ea4cacbbcdd78e9e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018383"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="abeb8-103">Aktualisieren von „managedAppPolicyDeploymentSummary“</span><span class="sxs-lookup"><span data-stu-id="abeb8-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="abeb8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="abeb8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abeb8-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="abeb8-105">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abeb8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="abeb8-106">Prerequisites</span></span>
<span data-ttu-id="abeb8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abeb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abeb8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="abeb8-109">Permission type</span></span>|<span data-ttu-id="abeb8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="abeb8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abeb8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="abeb8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="abeb8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abeb8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="abeb8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="abeb8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abeb8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abeb8-114">Not supported.</span></span>|
|<span data-ttu-id="abeb8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="abeb8-115">Application</span></span>|<span data-ttu-id="abeb8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="abeb8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abeb8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="abeb8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="request-headers"></a><span data-ttu-id="abeb8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="abeb8-118">Request headers</span></span>
|<span data-ttu-id="abeb8-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="abeb8-119">Header</span></span>|<span data-ttu-id="abeb8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="abeb8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abeb8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="abeb8-121">Authorization</span></span>|<span data-ttu-id="abeb8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="abeb8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abeb8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="abeb8-123">Accept</span></span>|<span data-ttu-id="abeb8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="abeb8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abeb8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="abeb8-125">Request body</span></span>
<span data-ttu-id="abeb8-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="abeb8-126">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="abeb8-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="abeb8-127">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="abeb8-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="abeb8-128">Property</span></span>|<span data-ttu-id="abeb8-129">Typ</span><span class="sxs-lookup"><span data-stu-id="abeb8-129">Type</span></span>|<span data-ttu-id="abeb8-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="abeb8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abeb8-131">displayName</span><span class="sxs-lookup"><span data-stu-id="abeb8-131">displayName</span></span>|<span data-ttu-id="abeb8-132">String</span><span class="sxs-lookup"><span data-stu-id="abeb8-132">String</span></span>|<span data-ttu-id="abeb8-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="abeb8-133">Not yet documented</span></span>|
|<span data-ttu-id="abeb8-134">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="abeb8-134">configurationDeployedUserCount</span></span>|<span data-ttu-id="abeb8-135">Int32</span><span class="sxs-lookup"><span data-stu-id="abeb8-135">Int32</span></span>|<span data-ttu-id="abeb8-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="abeb8-136">Not yet documented</span></span>|
|<span data-ttu-id="abeb8-137">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="abeb8-137">lastRefreshTime</span></span>|<span data-ttu-id="abeb8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="abeb8-138">DateTimeOffset</span></span>|<span data-ttu-id="abeb8-139">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="abeb8-139">Not yet documented</span></span>|
|<span data-ttu-id="abeb8-140">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="abeb8-140">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="abeb8-141">Collection von Objekten des Typs [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="abeb8-141">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="abeb8-142">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="abeb8-142">Not yet documented</span></span>|
|<span data-ttu-id="abeb8-143">id</span><span class="sxs-lookup"><span data-stu-id="abeb8-143">id</span></span>|<span data-ttu-id="abeb8-144">String</span><span class="sxs-lookup"><span data-stu-id="abeb8-144">String</span></span>|<span data-ttu-id="abeb8-145">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="abeb8-145">Key of the entity.</span></span>|
|<span data-ttu-id="abeb8-146">Version</span><span class="sxs-lookup"><span data-stu-id="abeb8-146">version</span></span>|<span data-ttu-id="abeb8-147">String</span><span class="sxs-lookup"><span data-stu-id="abeb8-147">String</span></span>|<span data-ttu-id="abeb8-148">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="abeb8-148">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="abeb8-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="abeb8-149">Response</span></span>
<span data-ttu-id="abeb8-150">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="abeb8-150">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abeb8-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="abeb8-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="abeb8-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="abeb8-152">Request</span></span>
<span data-ttu-id="abeb8-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="abeb8-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 588

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="abeb8-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="abeb8-154">Response</span></span>
<span data-ttu-id="abeb8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="abeb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 637

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
  "version": "Version value"
}
```



