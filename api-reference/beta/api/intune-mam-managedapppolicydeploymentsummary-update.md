---
title: Aktualisieren von „managedAppPolicyDeploymentSummary“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedAppPolicyDeploymentSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d68bb17015f21a479c014ab9df9d9ac2545faf9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30965984"
---
# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="27615-103">Aktualisieren von „managedAppPolicyDeploymentSummary“</span><span class="sxs-lookup"><span data-stu-id="27615-103">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="27615-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="27615-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27615-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="27615-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27615-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span><span class="sxs-lookup"><span data-stu-id="27615-106">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27615-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="27615-107">Prerequisites</span></span>
<span data-ttu-id="27615-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27615-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27615-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="27615-110">Permission type</span></span>|<span data-ttu-id="27615-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="27615-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27615-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="27615-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27615-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27615-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="27615-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="27615-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27615-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27615-115">Not supported.</span></span>|
|<span data-ttu-id="27615-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="27615-116">Application</span></span>|<span data-ttu-id="27615-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27615-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27615-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="27615-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="27615-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="27615-119">Request headers</span></span>
|<span data-ttu-id="27615-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="27615-120">Header</span></span>|<span data-ttu-id="27615-121">Wert</span><span class="sxs-lookup"><span data-stu-id="27615-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27615-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27615-122">Authorization</span></span>|<span data-ttu-id="27615-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="27615-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27615-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="27615-124">Accept</span></span>|<span data-ttu-id="27615-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27615-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27615-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="27615-126">Request body</span></span>
<span data-ttu-id="27615-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) an.</span><span class="sxs-lookup"><span data-stu-id="27615-127">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="27615-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="27615-128">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="27615-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27615-129">Property</span></span>|<span data-ttu-id="27615-130">Typ</span><span class="sxs-lookup"><span data-stu-id="27615-130">Type</span></span>|<span data-ttu-id="27615-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27615-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27615-132">displayName</span><span class="sxs-lookup"><span data-stu-id="27615-132">displayName</span></span>|<span data-ttu-id="27615-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="27615-133">String</span></span>|<span data-ttu-id="27615-134">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="27615-134">Not yet documented</span></span>|
|<span data-ttu-id="27615-135">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="27615-135">configurationDeployedUserCount</span></span>|<span data-ttu-id="27615-136">Int32</span><span class="sxs-lookup"><span data-stu-id="27615-136">Int32</span></span>|<span data-ttu-id="27615-137">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="27615-137">Not yet documented</span></span>|
|<span data-ttu-id="27615-138">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="27615-138">lastRefreshTime</span></span>|<span data-ttu-id="27615-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27615-139">DateTimeOffset</span></span>|<span data-ttu-id="27615-140">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="27615-140">Not yet documented</span></span>|
|<span data-ttu-id="27615-141">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="27615-141">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="27615-142">Collection von Objekten des Typs [managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md)</span><span class="sxs-lookup"><span data-stu-id="27615-142">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune-mam-managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="27615-143">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="27615-143">Not yet documented</span></span>|
|<span data-ttu-id="27615-144">id</span><span class="sxs-lookup"><span data-stu-id="27615-144">id</span></span>|<span data-ttu-id="27615-145">String</span><span class="sxs-lookup"><span data-stu-id="27615-145">String</span></span>|<span data-ttu-id="27615-146">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="27615-146">Key of the entity.</span></span>|
|<span data-ttu-id="27615-147">Version</span><span class="sxs-lookup"><span data-stu-id="27615-147">version</span></span>|<span data-ttu-id="27615-148">String</span><span class="sxs-lookup"><span data-stu-id="27615-148">String</span></span>|<span data-ttu-id="27615-149">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="27615-149">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="27615-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="27615-150">Response</span></span>
<span data-ttu-id="27615-151">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="27615-151">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune-mam-managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27615-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="27615-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="27615-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="27615-153">Request</span></span>
<span data-ttu-id="27615-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="27615-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
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

### <a name="response"></a><span data-ttu-id="27615-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="27615-155">Response</span></span>
<span data-ttu-id="27615-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="27615-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




