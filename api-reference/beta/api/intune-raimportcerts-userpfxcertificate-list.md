---
title: Liste userPFXCertificates
description: Listeneigenschaften und Beziehungen der UserPFXCertificate-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2f186842a5dc22a6fd43472b421988e4babb1fb9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940330"
---
# <a name="list-userpfxcertificates"></a><span data-ttu-id="a50d9-103">Liste userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="a50d9-103">List userPFXCertificates</span></span>

> <span data-ttu-id="a50d9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a50d9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a50d9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a50d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a50d9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a50d9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a50d9-107">Listeneigenschaften und Beziehungen der [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="a50d9-107">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a50d9-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a50d9-108">Prerequisites</span></span>
<span data-ttu-id="a50d9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a50d9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a50d9-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a50d9-111">Permission type</span></span>|<span data-ttu-id="a50d9-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a50d9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a50d9-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a50d9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a50d9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a50d9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a50d9-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a50d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a50d9-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a50d9-116">Not supported.</span></span>|
|<span data-ttu-id="a50d9-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a50d9-117">Application</span></span>|<span data-ttu-id="a50d9-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a50d9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a50d9-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a50d9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="a50d9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a50d9-120">Request headers</span></span>
|<span data-ttu-id="a50d9-121">Header</span><span class="sxs-lookup"><span data-stu-id="a50d9-121">Header</span></span>|<span data-ttu-id="a50d9-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a50d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a50d9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a50d9-123">Authorization</span></span>|<span data-ttu-id="a50d9-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a50d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a50d9-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a50d9-125">Accept</span></span>|<span data-ttu-id="a50d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a50d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a50d9-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a50d9-127">Request body</span></span>
<span data-ttu-id="a50d9-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a50d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a50d9-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a50d9-129">Response</span></span>
<span data-ttu-id="a50d9-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [UserPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="a50d9-130">If successful, this method returns a `200 OK` response code and a collection of [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a50d9-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a50d9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a50d9-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a50d9-132">Request</span></span>
<span data-ttu-id="a50d9-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a50d9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
```

### <a name="response"></a><span data-ttu-id="a50d9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a50d9-134">Response</span></span>
<span data-ttu-id="a50d9-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a50d9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 784

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userPFXCertificate",
      "id": "045c159b-159b-045c-9b15-5c049b155c04",
      "thumbprint": "Thumbprint value",
      "intendedPurpose": "smimeEncryption",
      "userPrincipalName": "User Principal Name value",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "providerName": "Provider Name value",
      "keyName": "Key Name value",
      "paddingScheme": "pkcs1",
      "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
      "encryptedPfxPassword": "Encrypted Pfx Password value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```





