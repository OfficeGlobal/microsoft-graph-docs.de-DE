---
title: Abrufen von windows10ImportedPFXCertificateProfile
description: Lesen Sie Eigenschaften und Beziehungen des windows10ImportedPFXCertificateProfile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 617c528eafd103b410e07c47ef276bf6b3b7339e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921290"
---
# <a name="get-windows10importedpfxcertificateprofile"></a><span data-ttu-id="93255-103">Abrufen von windows10ImportedPFXCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="93255-103">Get windows10ImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="93255-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="93255-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93255-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="93255-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="93255-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="93255-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93255-107">Lesen Sie Eigenschaften und Beziehungen des [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="93255-107">Read properties and relationships of the [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="93255-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="93255-108">Prerequisites</span></span>
<span data-ttu-id="93255-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93255-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93255-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="93255-111">Permission type</span></span>|<span data-ttu-id="93255-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="93255-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93255-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="93255-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93255-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="93255-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="93255-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="93255-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93255-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93255-116">Not supported.</span></span>|
|<span data-ttu-id="93255-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="93255-117">Application</span></span>|<span data-ttu-id="93255-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="93255-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93255-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="93255-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93255-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="93255-120">Optional query parameters</span></span>
<span data-ttu-id="93255-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="93255-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="93255-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="93255-122">Request headers</span></span>
|<span data-ttu-id="93255-123">Header</span><span class="sxs-lookup"><span data-stu-id="93255-123">Header</span></span>|<span data-ttu-id="93255-124">Wert</span><span class="sxs-lookup"><span data-stu-id="93255-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93255-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="93255-125">Authorization</span></span>|<span data-ttu-id="93255-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="93255-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93255-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="93255-127">Accept</span></span>|<span data-ttu-id="93255-128">application/json</span><span class="sxs-lookup"><span data-stu-id="93255-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93255-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="93255-129">Request body</span></span>
<span data-ttu-id="93255-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="93255-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93255-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="93255-131">Response</span></span>
<span data-ttu-id="93255-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="93255-132">If successful, this method returns a `200 OK` response code and [windows10ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windows10importedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93255-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="93255-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="93255-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="93255-134">Request</span></span>
<span data-ttu-id="93255-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="93255-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="93255-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="93255-136">Response</span></span>
<span data-ttu-id="93255-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="93255-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 813

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10ImportedPFXCertificateProfile",
    "id": "b582514b-514b-b582-4b51-82b54b5182b5",
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
    "certificateValidityPeriodScale": "months",
    "intendedPurpose": "smimeEncryption"
  }
}
```





