---
title: Erstellen von „deviceConfigurationUserStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceConfigurationUserStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2b4b0406de54604d09811f4034ae4e3883c91a3c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858569"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="af642-103">Erstellen von „deviceConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="af642-103">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="af642-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="af642-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af642-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="af642-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af642-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="af642-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af642-107">Diese Methode erstellt ein neues Objekt des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="af642-107">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af642-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="af642-108">Prerequisites</span></span>
<span data-ttu-id="af642-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af642-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af642-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="af642-111">Permission type</span></span>|<span data-ttu-id="af642-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="af642-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af642-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="af642-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af642-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af642-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="af642-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="af642-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af642-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af642-116">Not supported.</span></span>|
|<span data-ttu-id="af642-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="af642-117">Application</span></span>|<span data-ttu-id="af642-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="af642-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af642-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="af642-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="af642-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="af642-120">Request headers</span></span>
|<span data-ttu-id="af642-121">Header</span><span class="sxs-lookup"><span data-stu-id="af642-121">Header</span></span>|<span data-ttu-id="af642-122">Wert</span><span class="sxs-lookup"><span data-stu-id="af642-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af642-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af642-123">Authorization</span></span>|<span data-ttu-id="af642-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="af642-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af642-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="af642-125">Accept</span></span>|<span data-ttu-id="af642-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af642-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af642-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="af642-127">Request body</span></span>
<span data-ttu-id="af642-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceConfigurationUserStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="af642-128">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="af642-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceConfigurationUserStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="af642-129">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="af642-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="af642-130">Property</span></span>|<span data-ttu-id="af642-131">Typ</span><span class="sxs-lookup"><span data-stu-id="af642-131">Type</span></span>|<span data-ttu-id="af642-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="af642-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af642-133">id</span><span class="sxs-lookup"><span data-stu-id="af642-133">id</span></span>|<span data-ttu-id="af642-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af642-134">String</span></span>|<span data-ttu-id="af642-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="af642-135">Key of the entity.</span></span>|
|<span data-ttu-id="af642-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="af642-136">userDisplayName</span></span>|<span data-ttu-id="af642-137">String</span><span class="sxs-lookup"><span data-stu-id="af642-137">String</span></span>|<span data-ttu-id="af642-138">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="af642-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="af642-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="af642-139">devicesCount</span></span>|<span data-ttu-id="af642-140">Int32</span><span class="sxs-lookup"><span data-stu-id="af642-140">Int32</span></span>|<span data-ttu-id="af642-141">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="af642-141">Devices count for that user.</span></span>|
|<span data-ttu-id="af642-142">status</span><span class="sxs-lookup"><span data-stu-id="af642-142">status</span></span>|[<span data-ttu-id="af642-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="af642-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="af642-144">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="af642-144">Compliance status of the policy report.</span></span> <span data-ttu-id="af642-145">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="af642-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="af642-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="af642-146">lastReportedDateTime</span></span>|<span data-ttu-id="af642-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af642-147">DateTimeOffset</span></span>|<span data-ttu-id="af642-148">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="af642-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="af642-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="af642-149">userPrincipalName</span></span>|<span data-ttu-id="af642-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="af642-150">String</span></span>|<span data-ttu-id="af642-151">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="af642-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="af642-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="af642-152">Response</span></span>
<span data-ttu-id="af642-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="af642-153">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af642-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="af642-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="af642-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="af642-155">Request</span></span>
<span data-ttu-id="af642-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="af642-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="af642-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="af642-157">Response</span></span>
<span data-ttu-id="af642-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="af642-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





