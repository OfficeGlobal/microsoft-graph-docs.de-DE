---
title: Aktualisieren von „deviceConfigurationUserStatus“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa2c02f24c33feab3a7a64c2d994f4bbc9943bdc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142070"
---
# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="b9bd9-103">Aktualisieren von „deviceConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="b9bd9-103">Update deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="b9bd9-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9bd9-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9bd9-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="b9bd9-106">Update the properties of a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9bd9-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b9bd9-107">Prerequisites</span></span>
<span data-ttu-id="b9bd9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b9bd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b9bd9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b9bd9-110">Permission type</span></span>|<span data-ttu-id="b9bd9-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b9bd9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9bd9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b9bd9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9bd9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9bd9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9bd9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b9bd9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9bd9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9bd9-115">Not supported.</span></span>|
|<span data-ttu-id="b9bd9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b9bd9-116">Application</span></span>|<span data-ttu-id="b9bd9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b9bd9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9bd9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9bd9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b9bd9-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b9bd9-119">Request headers</span></span>
|<span data-ttu-id="b9bd9-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b9bd9-120">Header</span></span>|<span data-ttu-id="b9bd9-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b9bd9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9bd9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9bd9-122">Authorization</span></span>|<span data-ttu-id="b9bd9-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b9bd9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9bd9-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b9bd9-124">Accept</span></span>|<span data-ttu-id="b9bd9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9bd9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9bd9-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b9bd9-126">Request body</span></span>
<span data-ttu-id="b9bd9-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) an.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-127">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="b9bd9-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-128">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="b9bd9-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b9bd9-129">Property</span></span>|<span data-ttu-id="b9bd9-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b9bd9-130">Type</span></span>|<span data-ttu-id="b9bd9-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b9bd9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9bd9-132">id</span><span class="sxs-lookup"><span data-stu-id="b9bd9-132">id</span></span>|<span data-ttu-id="b9bd9-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9bd9-133">String</span></span>|<span data-ttu-id="b9bd9-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="b9bd9-134">Key of the entity.</span></span>|
|<span data-ttu-id="b9bd9-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b9bd9-135">userDisplayName</span></span>|<span data-ttu-id="b9bd9-136">String</span><span class="sxs-lookup"><span data-stu-id="b9bd9-136">String</span></span>|<span data-ttu-id="b9bd9-137">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="b9bd9-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b9bd9-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="b9bd9-138">devicesCount</span></span>|<span data-ttu-id="b9bd9-139">Int32</span><span class="sxs-lookup"><span data-stu-id="b9bd9-139">Int32</span></span>|<span data-ttu-id="b9bd9-140">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="b9bd9-140">Devices count for that user.</span></span>|
|<span data-ttu-id="b9bd9-141">status</span><span class="sxs-lookup"><span data-stu-id="b9bd9-141">status</span></span>|[<span data-ttu-id="b9bd9-142">Wurde</span><span class="sxs-lookup"><span data-stu-id="b9bd9-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b9bd9-143">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-143">Compliance status of the policy report.</span></span> <span data-ttu-id="b9bd9-144">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b9bd9-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9bd9-145">lastReportedDateTime</span></span>|<span data-ttu-id="b9bd9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9bd9-146">DateTimeOffset</span></span>|<span data-ttu-id="b9bd9-147">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="b9bd9-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b9bd9-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9bd9-148">userPrincipalName</span></span>|<span data-ttu-id="b9bd9-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b9bd9-149">String</span></span>|<span data-ttu-id="b9bd9-150">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="b9bd9-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b9bd9-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9bd9-151">Response</span></span>
<span data-ttu-id="b9bd9-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-152">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9bd9-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b9bd9-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9bd9-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b9bd9-154">Request</span></span>
<span data-ttu-id="b9bd9-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="b9bd9-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="b9bd9-156">Response</span></span>
<span data-ttu-id="b9bd9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b9bd9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




