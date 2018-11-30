---
title: Abrufen von macOSScepCertificateProfile
description: Lesen Sie Eigenschaften und Beziehungen des MacOSScepCertificateProfile-Objekts.
ms.openlocfilehash: a5d3d274c55e1b0da69aaa3158a61a2a7b7b1355
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064884"
---
# <a name="get-macosscepcertificateprofile"></a><span data-ttu-id="36c93-103">Abrufen von macOSScepCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="36c93-103">Get macOSScepCertificateProfile</span></span>

> <span data-ttu-id="36c93-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="36c93-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36c93-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="36c93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36c93-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="36c93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36c93-107">Lesen Sie Eigenschaften und Beziehungen des [MacOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="36c93-107">Read properties and relationships of the [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36c93-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="36c93-108">Prerequisites</span></span>
<span data-ttu-id="36c93-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36c93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36c93-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="36c93-111">Permission type</span></span>|<span data-ttu-id="36c93-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="36c93-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36c93-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="36c93-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36c93-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="36c93-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="36c93-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="36c93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36c93-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36c93-116">Not supported.</span></span>|
|<span data-ttu-id="36c93-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="36c93-117">Application</span></span>|<span data-ttu-id="36c93-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="36c93-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36c93-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="36c93-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36c93-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="36c93-120">Optional query parameters</span></span>
<span data-ttu-id="36c93-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="36c93-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="36c93-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="36c93-122">Request headers</span></span>
|<span data-ttu-id="36c93-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="36c93-123">Header</span></span>|<span data-ttu-id="36c93-124">Wert</span><span class="sxs-lookup"><span data-stu-id="36c93-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36c93-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="36c93-125">Authorization</span></span>|<span data-ttu-id="36c93-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="36c93-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36c93-127">Accept</span><span class="sxs-lookup"><span data-stu-id="36c93-127">Accept</span></span>|<span data-ttu-id="36c93-128">application/json</span><span class="sxs-lookup"><span data-stu-id="36c93-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36c93-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="36c93-129">Request body</span></span>
<span data-ttu-id="36c93-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="36c93-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36c93-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="36c93-131">Response</span></span>
<span data-ttu-id="36c93-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [MacOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="36c93-132">If successful, this method returns a `200 OK` response code and [macOSScepCertificateProfile](../resources/intune-deviceconfig-macosscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36c93-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="36c93-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="36c93-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="36c93-134">Request</span></span>
<span data-ttu-id="36c93-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36c93-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="36c93-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="36c93-136">Response</span></span>
<span data-ttu-id="36c93-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="36c93-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1218

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSScepCertificateProfile",
    "id": "78c3929d-929d-78c3-9d92-c3789d92c378",
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
    "subjectNameFormat": "commonNameAsEmail",
    "subjectAlternativeNameType": "emailAddress",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months",
    "scepServerUrls": [
      "Scep Server Urls value"
    ],
    "subjectNameFormatString": "Subject Name Format String value",
    "keyUsage": "digitalSignature",
    "keySize": "size2048",
    "hashAlgorithm": "sha2",
    "extendedKeyUsages": [
      {
        "@odata.type": "microsoft.graph.extendedKeyUsage",
        "name": "Name value",
        "objectIdentifier": "Object Identifier value"
      }
    ],
    "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
  }
}
```





