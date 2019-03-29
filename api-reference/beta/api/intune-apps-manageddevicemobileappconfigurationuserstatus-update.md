---
title: Aktualisieren von „managedDeviceMobileAppConfigurationUserStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs managedDeviceMobileAppConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cf319bfa8e0f1126d5f15b5c253962914b7bcb56
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962855"
---
# <a name="update-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="2ce66-103">Aktualisieren von „managedDeviceMobileAppConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="2ce66-103">Update managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="2ce66-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2ce66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ce66-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="2ce66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ce66-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="2ce66-106">Update the properties of a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ce66-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2ce66-107">Prerequisites</span></span>
<span data-ttu-id="2ce66-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ce66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ce66-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2ce66-110">Permission type</span></span>|<span data-ttu-id="2ce66-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2ce66-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ce66-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2ce66-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ce66-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ce66-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2ce66-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2ce66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ce66-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ce66-115">Not supported.</span></span>|
|<span data-ttu-id="2ce66-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2ce66-116">Application</span></span>|<span data-ttu-id="2ce66-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2ce66-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ce66-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ce66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="2ce66-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2ce66-119">Request headers</span></span>
|<span data-ttu-id="2ce66-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2ce66-120">Header</span></span>|<span data-ttu-id="2ce66-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2ce66-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ce66-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ce66-122">Authorization</span></span>|<span data-ttu-id="2ce66-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2ce66-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ce66-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2ce66-124">Accept</span></span>|<span data-ttu-id="2ce66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ce66-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ce66-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2ce66-126">Request body</span></span>
<span data-ttu-id="2ce66-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="2ce66-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="2ce66-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="2ce66-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="2ce66-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2ce66-129">Property</span></span>|<span data-ttu-id="2ce66-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2ce66-130">Type</span></span>|<span data-ttu-id="2ce66-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ce66-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ce66-132">id</span><span class="sxs-lookup"><span data-stu-id="2ce66-132">id</span></span>|<span data-ttu-id="2ce66-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ce66-133">String</span></span>|<span data-ttu-id="2ce66-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="2ce66-134">Key of the entity.</span></span>|
|<span data-ttu-id="2ce66-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2ce66-135">userDisplayName</span></span>|<span data-ttu-id="2ce66-136">String</span><span class="sxs-lookup"><span data-stu-id="2ce66-136">String</span></span>|<span data-ttu-id="2ce66-137">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="2ce66-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2ce66-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="2ce66-138">devicesCount</span></span>|<span data-ttu-id="2ce66-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2ce66-139">Int32</span></span>|<span data-ttu-id="2ce66-140">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="2ce66-140">Devices count for that user.</span></span>|
|<span data-ttu-id="2ce66-141">status</span><span class="sxs-lookup"><span data-stu-id="2ce66-141">status</span></span>|[<span data-ttu-id="2ce66-142">Wurde</span><span class="sxs-lookup"><span data-stu-id="2ce66-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2ce66-143">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="2ce66-143">Compliance status of the policy report.</span></span> <span data-ttu-id="2ce66-144">Mögliche Werte: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2ce66-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2ce66-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ce66-145">lastReportedDateTime</span></span>|<span data-ttu-id="2ce66-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ce66-146">DateTimeOffset</span></span>|<span data-ttu-id="2ce66-147">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="2ce66-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2ce66-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2ce66-148">userPrincipalName</span></span>|<span data-ttu-id="2ce66-149">String</span><span class="sxs-lookup"><span data-stu-id="2ce66-149">String</span></span>|<span data-ttu-id="2ce66-150">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="2ce66-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2ce66-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ce66-151">Response</span></span>
<span data-ttu-id="2ce66-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2ce66-152">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ce66-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2ce66-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ce66-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2ce66-154">Request</span></span>
<span data-ttu-id="2ce66-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2ce66-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="2ce66-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="2ce66-156">Response</span></span>
<span data-ttu-id="2ce66-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2ce66-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
  "id": "44960944-0944-4496-4409-964444099644",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




