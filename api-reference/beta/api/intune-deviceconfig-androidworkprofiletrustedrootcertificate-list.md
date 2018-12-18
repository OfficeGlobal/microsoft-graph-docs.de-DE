---
title: Liste androidWorkProfileTrustedRootCertificates
description: Listeneigenschaften und Beziehungen der AndroidWorkProfileTrustedRootCertificate-Objekte.
author: tfitzmac
ms.openlocfilehash: 87fd15f1e97e7924abbae4fc47537e298058788d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355121"
---
# <a name="list-androidworkprofiletrustedrootcertificates"></a><span data-ttu-id="40543-103">Liste androidWorkProfileTrustedRootCertificates</span><span class="sxs-lookup"><span data-stu-id="40543-103">List androidWorkProfileTrustedRootCertificates</span></span>

> <span data-ttu-id="40543-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="40543-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40543-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40543-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40543-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="40543-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40543-107">Listeneigenschaften und Beziehungen der [AndroidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="40543-107">List properties and relationships of the [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40543-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="40543-108">Prerequisites</span></span>
<span data-ttu-id="40543-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40543-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40543-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40543-111">Permission type</span></span>|<span data-ttu-id="40543-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40543-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40543-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40543-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40543-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="40543-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="40543-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40543-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40543-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40543-116">Not supported.</span></span>|
|<span data-ttu-id="40543-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40543-117">Application</span></span>|<span data-ttu-id="40543-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="40543-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40543-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40543-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="40543-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40543-120">Request headers</span></span>
|<span data-ttu-id="40543-121">Header</span><span class="sxs-lookup"><span data-stu-id="40543-121">Header</span></span>|<span data-ttu-id="40543-122">Wert</span><span class="sxs-lookup"><span data-stu-id="40543-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40543-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="40543-123">Authorization</span></span>|<span data-ttu-id="40543-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="40543-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40543-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40543-125">Accept</span></span>|<span data-ttu-id="40543-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40543-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40543-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40543-127">Request body</span></span>
<span data-ttu-id="40543-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="40543-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40543-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="40543-129">Response</span></span>
<span data-ttu-id="40543-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [AndroidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="40543-130">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40543-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40543-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="40543-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40543-132">Request</span></span>
<span data-ttu-id="40543-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40543-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="40543-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="40543-134">Response</span></span>
<span data-ttu-id="40543-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40543-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 635

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileTrustedRootCertificate",
      "id": "37cc7454-7454-37cc-5474-cc375474cc37",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
      "certFileName": "Cert File Name value"
    }
  ]
}
```





