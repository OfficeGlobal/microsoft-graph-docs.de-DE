---
title: Liste iosPkcsCertificateProfiles
description: Listeneigenschaften und Beziehungen der IosPkcsCertificateProfile-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43a189dc82a0de55ef8aac3eb4e568edceb700c9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955051"
---
# <a name="list-iospkcscertificateprofiles"></a><span data-ttu-id="aaeaa-103">Liste iosPkcsCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="aaeaa-103">List iosPkcsCertificateProfiles</span></span>

> <span data-ttu-id="aaeaa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="aaeaa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aaeaa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="aaeaa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aaeaa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="aaeaa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aaeaa-107">Listeneigenschaften und Beziehungen der [IosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="aaeaa-107">List properties and relationships of the [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aaeaa-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="aaeaa-108">Prerequisites</span></span>
<span data-ttu-id="aaeaa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaeaa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaeaa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aaeaa-111">Permission type</span></span>|<span data-ttu-id="aaeaa-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aaeaa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaeaa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aaeaa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aaeaa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aaeaa-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="aaeaa-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aaeaa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaeaa-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aaeaa-116">Not supported.</span></span>|
|<span data-ttu-id="aaeaa-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aaeaa-117">Application</span></span>|<span data-ttu-id="aaeaa-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="aaeaa-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaeaa-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aaeaa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="aaeaa-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aaeaa-120">Request headers</span></span>
|<span data-ttu-id="aaeaa-121">Header</span><span class="sxs-lookup"><span data-stu-id="aaeaa-121">Header</span></span>|<span data-ttu-id="aaeaa-122">Wert</span><span class="sxs-lookup"><span data-stu-id="aaeaa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaeaa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaeaa-123">Authorization</span></span>|<span data-ttu-id="aaeaa-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="aaeaa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaeaa-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="aaeaa-125">Accept</span></span>|<span data-ttu-id="aaeaa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aaeaa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaeaa-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aaeaa-127">Request body</span></span>
<span data-ttu-id="aaeaa-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="aaeaa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaeaa-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="aaeaa-129">Response</span></span>
<span data-ttu-id="aaeaa-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [IosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="aaeaa-130">If successful, this method returns a `200 OK` response code and a collection of [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaeaa-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="aaeaa-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="aaeaa-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aaeaa-132">Request</span></span>
<span data-ttu-id="aaeaa-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aaeaa-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="aaeaa-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="aaeaa-134">Response</span></span>
<span data-ttu-id="aaeaa-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aaeaa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1046

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosPkcsCertificateProfile",
      "id": "ed0264dd-64dd-ed02-dd64-02eddd6402ed",
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
      "certificationAuthority": "Certification Authority value",
      "certificationAuthorityName": "Certification Authority Name value",
      "certificateTemplateName": "Certificate Template Name value",
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
    }
  ]
}
```





