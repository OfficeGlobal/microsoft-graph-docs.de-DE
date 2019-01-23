---
title: Abrufen von androidPkcsCertificateProfile
description: Lesen Sie Eigenschaften und Beziehungen des AndroidPkcsCertificateProfile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5e925f9c6d786934c18e9f75e1a332b32440ab8a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413276"
---
# <a name="get-androidpkcscertificateprofile"></a><span data-ttu-id="b68b8-103">Abrufen von androidPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="b68b8-103">Get androidPkcsCertificateProfile</span></span>

> <span data-ttu-id="b68b8-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b68b8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b68b8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b68b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b68b8-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b68b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b68b8-107">Lesen Sie Eigenschaften und Beziehungen des [AndroidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b68b8-107">Read properties and relationships of the [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b68b8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b68b8-108">Prerequisites</span></span>
<span data-ttu-id="b68b8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b68b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b68b8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b68b8-111">Permission type</span></span>|<span data-ttu-id="b68b8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b68b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b68b8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b68b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b68b8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b68b8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b68b8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b68b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b68b8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b68b8-116">Not supported.</span></span>|
|<span data-ttu-id="b68b8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b68b8-117">Application</span></span>|<span data-ttu-id="b68b8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b68b8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b68b8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b68b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b68b8-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b68b8-120">Optional query parameters</span></span>
<span data-ttu-id="b68b8-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b68b8-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b68b8-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b68b8-122">Request headers</span></span>
|<span data-ttu-id="b68b8-123">Header</span><span class="sxs-lookup"><span data-stu-id="b68b8-123">Header</span></span>|<span data-ttu-id="b68b8-124">Wert</span><span class="sxs-lookup"><span data-stu-id="b68b8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b68b8-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b68b8-125">Authorization</span></span>|<span data-ttu-id="b68b8-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b68b8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b68b8-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b68b8-127">Accept</span></span>|<span data-ttu-id="b68b8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b68b8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b68b8-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b68b8-129">Request body</span></span>
<span data-ttu-id="b68b8-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b68b8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b68b8-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b68b8-131">Response</span></span>
<span data-ttu-id="b68b8-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="b68b8-132">If successful, this method returns a `200 OK` response code and [androidPkcsCertificateProfile](../resources/intune-deviceconfig-androidpkcscertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b68b8-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b68b8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="b68b8-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b68b8-134">Request</span></span>
<span data-ttu-id="b68b8-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b68b8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="b68b8-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b68b8-136">Response</span></span>
<span data-ttu-id="b68b8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b68b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1203

{
  "value": {
    "@odata.type": "#microsoft.graph.androidPkcsCertificateProfile",
    "id": "bb55705b-705b-bb55-5b70-55bb5b7055bb",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "renewalThresholdPercentage": 10,
    "subjectNameFormat": "commonNameIncludingEmail",
    "subjectAlternativeNameType": "emailAddress",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "certificationAuthority": "Certification Authority value",
    "certificationAuthorityName": "Certification Authority Name value",
    "certificateTemplateName": "Certificate Template Name value",
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
  }
}
```




