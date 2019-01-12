---
title: Abrufen von windows10CertificateProfileBase
description: Lesen Sie Eigenschaften und Beziehungen des windows10CertificateProfileBase-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1e9596cc1cfacd89435394f5db62bf1a2a3e3e87
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984402"
---
# <a name="get-windows10certificateprofilebase"></a><span data-ttu-id="5a013-103">Abrufen von windows10CertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="5a013-103">Get windows10CertificateProfileBase</span></span>

> <span data-ttu-id="5a013-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5a013-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a013-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5a013-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a013-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5a013-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a013-107">Lesen Sie Eigenschaften und Beziehungen des [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5a013-107">Read properties and relationships of the [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a013-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5a013-108">Prerequisites</span></span>
<span data-ttu-id="5a013-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a013-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a013-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5a013-111">Permission type</span></span>|<span data-ttu-id="5a013-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5a013-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a013-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5a013-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a013-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5a013-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5a013-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5a013-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a013-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a013-116">Not supported.</span></span>|
|<span data-ttu-id="5a013-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5a013-117">Application</span></span>|<span data-ttu-id="5a013-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5a013-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a013-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a013-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5a013-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5a013-120">Optional query parameters</span></span>
<span data-ttu-id="5a013-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5a013-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5a013-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5a013-122">Request headers</span></span>
|<span data-ttu-id="5a013-123">Header</span><span class="sxs-lookup"><span data-stu-id="5a013-123">Header</span></span>|<span data-ttu-id="5a013-124">Wert</span><span class="sxs-lookup"><span data-stu-id="5a013-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a013-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a013-125">Authorization</span></span>|<span data-ttu-id="5a013-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5a013-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a013-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5a013-127">Accept</span></span>|<span data-ttu-id="5a013-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5a013-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a013-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5a013-129">Request body</span></span>
<span data-ttu-id="5a013-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5a013-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5a013-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a013-131">Response</span></span>
<span data-ttu-id="5a013-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5a013-132">If successful, this method returns a `200 OK` response code and [windows10CertificateProfileBase](../resources/intune-deviceconfig-windows10certificateprofilebase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a013-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5a013-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a013-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5a013-134">Request</span></span>
<span data-ttu-id="5a013-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5a013-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5a013-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5a013-136">Response</span></span>
<span data-ttu-id="5a013-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5a013-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 763

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10CertificateProfileBase",
    "id": "1f01ffc6-ffc6-1f01-c6ff-011fc6ff011f",
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
    "keyStorageProvider": "useTpmKspOtherwiseFail",
    "subjectNameFormat": "commonNameIncludingEmail",
    "subjectAlternativeNameType": "emailAddress",
    "certificateValidityPeriodValue": 14,
    "certificateValidityPeriodScale": "months"
  }
}
```





