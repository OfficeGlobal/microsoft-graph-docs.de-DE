---
title: ManagedDeviceCertificateStates aufListen
description: AufListen von Eigenschaften und Beziehungen der managedDeviceCertificateState-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d3497a3641ff9823e94bd2bfb3ca77d99a4ef344
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146494"
---
# <a name="list-manageddevicecertificatestates"></a><span data-ttu-id="e00ec-103">ManagedDeviceCertificateStates aufListen</span><span class="sxs-lookup"><span data-stu-id="e00ec-103">List managedDeviceCertificateStates</span></span>

> <span data-ttu-id="e00ec-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e00ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e00ec-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e00ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e00ec-106">AufListen von Eigenschaften und Beziehungen der [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="e00ec-106">List properties and relationships of the [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e00ec-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e00ec-107">Prerequisites</span></span>
<span data-ttu-id="e00ec-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e00ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e00ec-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e00ec-110">Permission type</span></span>|<span data-ttu-id="e00ec-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e00ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e00ec-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e00ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e00ec-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e00ec-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e00ec-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e00ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e00ec-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e00ec-115">Not supported.</span></span>|
|<span data-ttu-id="e00ec-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e00ec-116">Application</span></span>|<span data-ttu-id="e00ec-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e00ec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e00ec-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e00ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="e00ec-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e00ec-119">Request headers</span></span>
|<span data-ttu-id="e00ec-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e00ec-120">Header</span></span>|<span data-ttu-id="e00ec-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e00ec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e00ec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e00ec-122">Authorization</span></span>|<span data-ttu-id="e00ec-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e00ec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e00ec-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e00ec-124">Accept</span></span>|<span data-ttu-id="e00ec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e00ec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e00ec-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e00ec-126">Request body</span></span>
<span data-ttu-id="e00ec-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e00ec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e00ec-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="e00ec-128">Response</span></span>
<span data-ttu-id="e00ec-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e00ec-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e00ec-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e00ec-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e00ec-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e00ec-131">Request</span></span>
<span data-ttu-id="e00ec-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e00ec-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
```

### <a name="response"></a><span data-ttu-id="e00ec-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e00ec-133">Response</span></span>
<span data-ttu-id="e00ec-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e00ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1703

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
      "id": "d99bc884-c884-d99b-84c8-9bd984c89bd9",
      "devicePlatform": "androidForWork",
      "certificateKeyUsage": "digitalSignature",
      "certificateValidityPeriodUnits": "months",
      "certificateIssuanceState": "challengeIssued",
      "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
      "certificateSubjectNameFormat": "commonNameIncludingEmail",
      "certificateSubjectAlternativeNameFormat": "emailAddress",
      "certificateRevokeStatus": "pending",
      "certificateProfileDisplayName": "Certificate Profile Display Name value",
      "deviceDisplayName": "Device Display Name value",
      "userDisplayName": "User Display Name value",
      "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
      "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
      "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
      "certificateIssuer": "Certificate Issuer value",
      "certificateThumbprint": "Certificate Thumbprint value",
      "certificateSerialNumber": "Certificate Serial Number value",
      "certificateKeyLength": 4,
      "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
      "certificateValidityPeriod": 9,
      "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
      "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
      "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
      "certificateErrorCode": 4
    }
  ]
}
```




