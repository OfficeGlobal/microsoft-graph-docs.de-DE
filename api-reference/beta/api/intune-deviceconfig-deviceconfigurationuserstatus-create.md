---
title: Erstellen von „deviceConfigurationUserStatus“
description: Diese Methode erstellt ein neues Objekt des Typs deviceConfigurationUserStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6792e4b428c00b798700c91887cefb672d315d34
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412268"
---
# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="4c686-103">Erstellen von „deviceConfigurationUserStatus“</span><span class="sxs-lookup"><span data-stu-id="4c686-103">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="4c686-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4c686-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4c686-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4c686-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c686-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4c686-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c686-107">Diese Methode erstellt ein neues Objekt des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="4c686-107">Create a new [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c686-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4c686-108">Prerequisites</span></span>
<span data-ttu-id="4c686-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c686-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4c686-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4c686-111">Permission type</span></span>|<span data-ttu-id="4c686-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4c686-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c686-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4c686-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c686-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c686-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c686-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4c686-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c686-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c686-116">Not supported.</span></span>|
|<span data-ttu-id="4c686-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4c686-117">Application</span></span>|<span data-ttu-id="4c686-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4c686-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c686-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c686-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4c686-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4c686-120">Request headers</span></span>
|<span data-ttu-id="4c686-121">Header</span><span class="sxs-lookup"><span data-stu-id="4c686-121">Header</span></span>|<span data-ttu-id="4c686-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4c686-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c686-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4c686-123">Authorization</span></span>|<span data-ttu-id="4c686-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4c686-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c686-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4c686-125">Accept</span></span>|<span data-ttu-id="4c686-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c686-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c686-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4c686-127">Request body</span></span>
<span data-ttu-id="4c686-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „deviceConfigurationUserStatus“ an.</span><span class="sxs-lookup"><span data-stu-id="4c686-128">In the request body, supply a JSON representation for the deviceConfigurationUserStatus object.</span></span>

<span data-ttu-id="4c686-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „deviceConfigurationUserStatus“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="4c686-129">The following table shows the properties that are required when you create the deviceConfigurationUserStatus.</span></span>

|<span data-ttu-id="4c686-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4c686-130">Property</span></span>|<span data-ttu-id="4c686-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4c686-131">Type</span></span>|<span data-ttu-id="4c686-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c686-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c686-133">id</span><span class="sxs-lookup"><span data-stu-id="4c686-133">id</span></span>|<span data-ttu-id="4c686-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c686-134">String</span></span>|<span data-ttu-id="4c686-135">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4c686-135">Key of the entity.</span></span>|
|<span data-ttu-id="4c686-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4c686-136">userDisplayName</span></span>|<span data-ttu-id="4c686-137">String</span><span class="sxs-lookup"><span data-stu-id="4c686-137">String</span></span>|<span data-ttu-id="4c686-138">Benutzername, der zu dem Objekt des Typs „DevicePolicyStatus“ gehört</span><span class="sxs-lookup"><span data-stu-id="4c686-138">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="4c686-139">devicesCount</span><span class="sxs-lookup"><span data-stu-id="4c686-139">devicesCount</span></span>|<span data-ttu-id="4c686-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4c686-140">Int32</span></span>|<span data-ttu-id="4c686-141">Geräteanzahl für den Benutzer</span><span class="sxs-lookup"><span data-stu-id="4c686-141">Devices count for that user.</span></span>|
|<span data-ttu-id="4c686-142">status</span><span class="sxs-lookup"><span data-stu-id="4c686-142">status</span></span>|[<span data-ttu-id="4c686-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4c686-143">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4c686-144">Konformitätsstatus des Richtlinienberichts.</span><span class="sxs-lookup"><span data-stu-id="4c686-144">Compliance status of the policy report.</span></span> <span data-ttu-id="4c686-145">Mögliche Werte sind: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict` und `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4c686-145">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4c686-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c686-146">lastReportedDateTime</span></span>|<span data-ttu-id="4c686-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c686-147">DateTimeOffset</span></span>|<span data-ttu-id="4c686-148">Datum und Uhrzeit der letzten Änderung des Richtlinienberichts</span><span class="sxs-lookup"><span data-stu-id="4c686-148">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="4c686-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4c686-149">userPrincipalName</span></span>|<span data-ttu-id="4c686-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c686-150">String</span></span>|<span data-ttu-id="4c686-151">Benutzerprinzipalname</span><span class="sxs-lookup"><span data-stu-id="4c686-151">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="4c686-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c686-152">Response</span></span>
<span data-ttu-id="4c686-153">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4c686-153">If successful, this method returns a `201 Created` response code and a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c686-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4c686-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c686-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4c686-155">Request</span></span>
<span data-ttu-id="4c686-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4c686-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c686-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="4c686-157">Response</span></span>
<span data-ttu-id="4c686-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4c686-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




