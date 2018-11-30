---
title: Liste androidScepCertificateProfiles
description: Listeneigenschaften und Beziehungen der AndroidScepCertificateProfile-Objekte.
ms.openlocfilehash: 425c00a28b5a7c584660941ddc951a05d54f0250
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061898"
---
# <a name="list-androidscepcertificateprofiles"></a><span data-ttu-id="92050-103">Liste androidScepCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="92050-103">List androidScepCertificateProfiles</span></span>

> <span data-ttu-id="92050-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="92050-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92050-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="92050-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="92050-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="92050-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92050-107">Listeneigenschaften und Beziehungen der [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="92050-107">List properties and relationships of the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="92050-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="92050-108">Prerequisites</span></span>
<span data-ttu-id="92050-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92050-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92050-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="92050-111">Permission type</span></span>|<span data-ttu-id="92050-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="92050-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92050-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="92050-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92050-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92050-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="92050-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="92050-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92050-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92050-116">Not supported.</span></span>|
|<span data-ttu-id="92050-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="92050-117">Application</span></span>|<span data-ttu-id="92050-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="92050-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92050-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="92050-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="92050-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="92050-120">Request headers</span></span>
|<span data-ttu-id="92050-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="92050-121">Header</span></span>|<span data-ttu-id="92050-122">Wert</span><span class="sxs-lookup"><span data-stu-id="92050-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92050-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="92050-123">Authorization</span></span>|<span data-ttu-id="92050-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="92050-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92050-125">Accept</span><span class="sxs-lookup"><span data-stu-id="92050-125">Accept</span></span>|<span data-ttu-id="92050-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92050-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92050-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="92050-127">Request body</span></span>
<span data-ttu-id="92050-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="92050-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92050-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="92050-129">Response</span></span>
<span data-ttu-id="92050-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="92050-130">If successful, this method returns a `200 OK` response code and a collection of [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92050-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="92050-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="92050-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="92050-132">Request</span></span>
<span data-ttu-id="92050-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="92050-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="92050-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="92050-134">Response</span></span>
<span data-ttu-id="92050-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="92050-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
      "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "hashAlgorithm": "sha2",
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
    }
  ]
}
```




