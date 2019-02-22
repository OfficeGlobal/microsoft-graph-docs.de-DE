---
title: Erstellen von „deviceConfigurationUserStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18294eacc11477bfe69eeec2ec15a84964313912
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144261"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="34fd1-103">Erstellen von „deviceConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="34fd1-103">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="34fd1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34fd1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34fd1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="34fd1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34fd1-106">Diese Methode erstellt ein neues Objekt des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="34fd1-106">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34fd1-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="34fd1-107">Prerequisites</span></span>
<span data-ttu-id="34fd1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="34fd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="34fd1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="34fd1-110">Permission type</span></span>|<span data-ttu-id="34fd1-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="34fd1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34fd1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="34fd1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34fd1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34fd1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34fd1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="34fd1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34fd1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34fd1-115">Not supported.</span></span>|
|<span data-ttu-id="34fd1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="34fd1-116">Application</span></span>|<span data-ttu-id="34fd1-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="34fd1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34fd1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="34fd1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="34fd1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="34fd1-119">Request headers</span></span>
|<span data-ttu-id="34fd1-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="34fd1-120">Header</span></span>|<span data-ttu-id="34fd1-121">Wert</span><span class="sxs-lookup"><span data-stu-id="34fd1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34fd1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="34fd1-122">Authorization</span></span>|<span data-ttu-id="34fd1-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="34fd1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34fd1-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="34fd1-124">Accept</span></span>|<span data-ttu-id="34fd1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34fd1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34fd1-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="34fd1-126">Request body</span></span>
<span data-ttu-id="34fd1-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceConfigurationUserStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="34fd1-127">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="34fd1-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceConfigurationUserStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="34fd1-128">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="34fd1-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="34fd1-129">Property</span></span>|<span data-ttu-id="34fd1-130">Typ</span><span class="sxs-lookup"><span data-stu-id="34fd1-130">Type</span></span>|<span data-ttu-id="34fd1-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34fd1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34fd1-132">id</span><span class="sxs-lookup"><span data-stu-id="34fd1-132">id</span></span>|<span data-ttu-id="34fd1-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34fd1-133">String</span></span>|<span data-ttu-id="34fd1-134">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="34fd1-134">Key of the entity.</span></span>|
|<span data-ttu-id="34fd1-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="34fd1-135">userDisplayName</span></span>|<span data-ttu-id="34fd1-136">String</span><span class="sxs-lookup"><span data-stu-id="34fd1-136">String</span></span>|<span data-ttu-id="34fd1-137">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="34fd1-137">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="34fd1-138">devicesCount</span><span class="sxs-lookup"><span data-stu-id="34fd1-138">devicesCount</span></span>|<span data-ttu-id="34fd1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="34fd1-139">Int32</span></span>|<span data-ttu-id="34fd1-140">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="34fd1-140">Devices count for that user.</span></span>|
|<span data-ttu-id="34fd1-141">status</span><span class="sxs-lookup"><span data-stu-id="34fd1-141">status</span></span>|[<span data-ttu-id="34fd1-142">Wurde</span><span class="sxs-lookup"><span data-stu-id="34fd1-142">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="34fd1-143">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="34fd1-143">Compliance status of the policy report.</span></span> <span data-ttu-id="34fd1-144">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="34fd1-144">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="34fd1-145">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="34fd1-145">lastReportedDateTime</span></span>|<span data-ttu-id="34fd1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34fd1-146">DateTimeOffset</span></span>|<span data-ttu-id="34fd1-147">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="34fd1-147">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="34fd1-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="34fd1-148">userPrincipalName</span></span>|<span data-ttu-id="34fd1-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34fd1-149">String</span></span>|<span data-ttu-id="34fd1-150">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="34fd1-150">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="34fd1-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="34fd1-151">Response</span></span>
<span data-ttu-id="34fd1-152">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="34fd1-152">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34fd1-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="34fd1-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="34fd1-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="34fd1-154">Request</span></span>
<span data-ttu-id="34fd1-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="34fd1-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="34fd1-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="34fd1-156">Response</span></span>
<span data-ttu-id="34fd1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="34fd1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




