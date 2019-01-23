---
title: Abrufen von androidWorkProfileCertificateProfileBase
description: Lesen Sie Eigenschaften und Beziehungen des AndroidWorkProfileCertificateProfileBase-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fbeb430b0ea5c365f2a74cce60b2719e545055f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418036"
---
# <a name="get-androidworkprofilecertificateprofilebase"></a><span data-ttu-id="c91f2-103">Abrufen von androidWorkProfileCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="c91f2-103">Get androidWorkProfileCertificateProfileBase</span></span>

> <span data-ttu-id="c91f2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c91f2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c91f2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c91f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c91f2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c91f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c91f2-107">Lesen Sie Eigenschaften und Beziehungen des [AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c91f2-107">Read properties and relationships of the [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c91f2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c91f2-108">Prerequisites</span></span>
<span data-ttu-id="c91f2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c91f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c91f2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c91f2-111">Permission type</span></span>|<span data-ttu-id="c91f2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c91f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c91f2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c91f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c91f2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c91f2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c91f2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c91f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c91f2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c91f2-116">Not supported.</span></span>|
|<span data-ttu-id="c91f2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c91f2-117">Application</span></span>|<span data-ttu-id="c91f2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c91f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c91f2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c91f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileVpnConfiguration/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEasEmailProfileBase/identityCertificate
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c91f2-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c91f2-120">Optional query parameters</span></span>
<span data-ttu-id="c91f2-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c91f2-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c91f2-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c91f2-122">Request headers</span></span>
|<span data-ttu-id="c91f2-123">Header</span><span class="sxs-lookup"><span data-stu-id="c91f2-123">Header</span></span>|<span data-ttu-id="c91f2-124">Wert</span><span class="sxs-lookup"><span data-stu-id="c91f2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c91f2-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c91f2-125">Authorization</span></span>|<span data-ttu-id="c91f2-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c91f2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c91f2-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c91f2-127">Accept</span></span>|<span data-ttu-id="c91f2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c91f2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c91f2-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c91f2-129">Request body</span></span>
<span data-ttu-id="c91f2-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c91f2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c91f2-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c91f2-131">Response</span></span>
<span data-ttu-id="c91f2-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [AndroidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c91f2-132">If successful, this method returns a `200 OK` response code and [androidWorkProfileCertificateProfileBase](../resources/intune-deviceconfig-androidworkprofilecertificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c91f2-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c91f2-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c91f2-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c91f2-134">Request</span></span>
<span data-ttu-id="c91f2-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c91f2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate
```

### <a name="response"></a><span data-ttu-id="c91f2-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c91f2-136">Response</span></span>
<span data-ttu-id="c91f2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c91f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 868

{
  "value": {
    "@odata.type": "#microsoft.graph.androidWorkProfileCertificateProfileBase",
    "id": "4a559c8b-9c8b-4a55-8b9c-554a8b9c554a",
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
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ]
  }
}
```




