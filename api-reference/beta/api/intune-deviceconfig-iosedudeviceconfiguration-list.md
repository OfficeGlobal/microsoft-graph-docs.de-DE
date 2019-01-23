---
title: Liste iosEduDeviceConfigurations
description: Listeneigenschaften und Beziehungen der IosEduDeviceConfiguration-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 04fec140f874aa287436a95f322f45c9bb89a644
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402188"
---
# <a name="list-iosedudeviceconfigurations"></a><span data-ttu-id="4b02d-103">Liste iosEduDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="4b02d-103">List iosEduDeviceConfigurations</span></span>

> <span data-ttu-id="4b02d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4b02d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4b02d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b02d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b02d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4b02d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b02d-107">Listeneigenschaften und Beziehungen der [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="4b02d-107">List properties and relationships of the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b02d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4b02d-108">Prerequisites</span></span>
<span data-ttu-id="4b02d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4b02d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4b02d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4b02d-111">Permission type</span></span>|<span data-ttu-id="4b02d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4b02d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b02d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4b02d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b02d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b02d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4b02d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4b02d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b02d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b02d-116">Not supported.</span></span>|
|<span data-ttu-id="4b02d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4b02d-117">Application</span></span>|<span data-ttu-id="4b02d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4b02d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b02d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b02d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4b02d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4b02d-120">Request headers</span></span>
|<span data-ttu-id="4b02d-121">Header</span><span class="sxs-lookup"><span data-stu-id="4b02d-121">Header</span></span>|<span data-ttu-id="4b02d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4b02d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b02d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4b02d-123">Authorization</span></span>|<span data-ttu-id="4b02d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4b02d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b02d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4b02d-125">Accept</span></span>|<span data-ttu-id="4b02d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b02d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b02d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4b02d-127">Request body</span></span>
<span data-ttu-id="4b02d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4b02d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b02d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b02d-129">Response</span></span>
<span data-ttu-id="4b02d-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4b02d-130">If successful, this method returns a `200 OK` response code and a collection of [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b02d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4b02d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b02d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4b02d-132">Request</span></span>
<span data-ttu-id="4b02d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4b02d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4b02d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4b02d-134">Response</span></span>
<span data-ttu-id="4b02d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4b02d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2291

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
      "id": "4c5df9b6-f9b6-4c5d-b6f9-5d4cb6f95d4c",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "teacherCertificateSettings": {
        "@odata.type": "microsoft.graph.iosEduCertificateSettings",
        "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
        "certFileName": "Cert File Name value",
        "certificationAuthority": "Certification Authority value",
        "certificationAuthorityName": "Certification Authority Name value",
        "certificateTemplateName": "Certificate Template Name value",
        "renewalThresholdPercentage": 10,
        "certificateValidityPeriodValue": 14,
        "certificateValidityPeriodScale": "months"
      },
      "studentCertificateSettings": {
        "@odata.type": "microsoft.graph.iosEduCertificateSettings",
        "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
        "certFileName": "Cert File Name value",
        "certificationAuthority": "Certification Authority value",
        "certificationAuthorityName": "Certification Authority Name value",
        "certificateTemplateName": "Certificate Template Name value",
        "renewalThresholdPercentage": 10,
        "certificateValidityPeriodValue": 14,
        "certificateValidityPeriodScale": "months"
      },
      "deviceCertificateSettings": {
        "@odata.type": "microsoft.graph.iosEduCertificateSettings",
        "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
        "certFileName": "Cert File Name value",
        "certificationAuthority": "Certification Authority value",
        "certificationAuthorityName": "Certification Authority Name value",
        "certificateTemplateName": "Certificate Template Name value",
        "renewalThresholdPercentage": 10,
        "certificateValidityPeriodValue": 14,
        "certificateValidityPeriodScale": "months"
      }
    }
  ]
}
```




