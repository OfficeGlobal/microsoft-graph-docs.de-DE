---
title: Aktualisieren von „managedAppPolicyDeploymentSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedAppPolicyDeploymentSummary.
ms.openlocfilehash: 2c0bf77e3dbd3720bcb0cfea28d69155174fb776
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066141"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="1fe9d-103">Aktualisieren von „managedAppPolicyDeploymentSummary“</span><span class="sxs-lookup"><span data-stu-id="1fe9d-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="1fe9d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1fe9d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fe9d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fe9d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1fe9d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1fe9d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1fe9d-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="1fe9d-107">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1fe9d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1fe9d-108">Prerequisites</span></span>
<span data-ttu-id="1fe9d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fe9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fe9d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1fe9d-111">Permission type</span></span>|<span data-ttu-id="1fe9d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1fe9d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1fe9d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1fe9d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1fe9d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fe9d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1fe9d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1fe9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1fe9d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1fe9d-116">Not supported.</span></span>|
|<span data-ttu-id="1fe9d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1fe9d-117">Application</span></span>|<span data-ttu-id="1fe9d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1fe9d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1fe9d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1fe9d-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1fe9d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1fe9d-120">Request headers</span></span>
|<span data-ttu-id="1fe9d-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1fe9d-121">Header</span></span>|<span data-ttu-id="1fe9d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1fe9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1fe9d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fe9d-123">Authorization</span></span>|<span data-ttu-id="1fe9d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1fe9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1fe9d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1fe9d-125">Accept</span></span>|<span data-ttu-id="1fe9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1fe9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fe9d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1fe9d-127">Request body</span></span>
<span data-ttu-id="1fe9d-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="1fe9d-128">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="1fe9d-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="1fe9d-129">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="1fe9d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1fe9d-130">Property</span></span>|<span data-ttu-id="1fe9d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1fe9d-131">Type</span></span>|<span data-ttu-id="1fe9d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1fe9d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fe9d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1fe9d-133">displayName</span></span>|<span data-ttu-id="1fe9d-134">String</span><span class="sxs-lookup"><span data-stu-id="1fe9d-134">String</span></span>|<span data-ttu-id="1fe9d-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1fe9d-135">Not yet documented</span></span>|
|<span data-ttu-id="1fe9d-136">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="1fe9d-136">configurationDeployedUserCount</span></span>|<span data-ttu-id="1fe9d-137">Int32</span><span class="sxs-lookup"><span data-stu-id="1fe9d-137">Int32</span></span>|<span data-ttu-id="1fe9d-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1fe9d-138">Not yet documented</span></span>|
|<span data-ttu-id="1fe9d-139">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="1fe9d-139">lastRefreshTime</span></span>|<span data-ttu-id="1fe9d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1fe9d-140">DateTimeOffset</span></span>|<span data-ttu-id="1fe9d-141">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1fe9d-141">Not yet documented</span></span>|
|<span data-ttu-id="1fe9d-142">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="1fe9d-142">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="1fe9d-143">Collection von Objekten des Typs [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="1fe9d-143">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="1fe9d-144">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="1fe9d-144">Not yet documented</span></span>|
|<span data-ttu-id="1fe9d-145">id</span><span class="sxs-lookup"><span data-stu-id="1fe9d-145">id</span></span>|<span data-ttu-id="1fe9d-146">String</span><span class="sxs-lookup"><span data-stu-id="1fe9d-146">String</span></span>|<span data-ttu-id="1fe9d-147">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1fe9d-147">Key of the entity.</span></span>|
|<span data-ttu-id="1fe9d-148">Version</span><span class="sxs-lookup"><span data-stu-id="1fe9d-148">version</span></span>|<span data-ttu-id="1fe9d-149">String</span><span class="sxs-lookup"><span data-stu-id="1fe9d-149">String</span></span>|<span data-ttu-id="1fe9d-150">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="1fe9d-150">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1fe9d-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="1fe9d-151">Response</span></span>
<span data-ttu-id="1fe9d-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1fe9d-152">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fe9d-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1fe9d-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="1fe9d-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1fe9d-154">Request</span></span>
<span data-ttu-id="1fe9d-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1fe9d-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 516

{
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

### <a name="response"></a><span data-ttu-id="1fe9d-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="1fe9d-156">Response</span></span>
<span data-ttu-id="1fe9d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1fe9d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





