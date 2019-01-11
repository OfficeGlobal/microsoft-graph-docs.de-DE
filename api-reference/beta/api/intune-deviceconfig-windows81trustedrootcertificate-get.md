---
title: Abrufen von windows81TrustedRootCertificate
description: Lesen Sie Eigenschaften und Beziehungen des windows81TrustedRootCertificate-Objekts.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 35bf33bcc9002e8b8f42d34a13ddcf52604297e0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842861"
---
# <a name="get-windows81trustedrootcertificate"></a><span data-ttu-id="17717-103">Abrufen von windows81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="17717-103">Get windows81TrustedRootCertificate</span></span>

> <span data-ttu-id="17717-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="17717-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17717-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="17717-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17717-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="17717-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17717-107">Lesen Sie Eigenschaften und Beziehungen des [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="17717-107">Read properties and relationships of the [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="17717-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="17717-108">Prerequisites</span></span>
<span data-ttu-id="17717-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17717-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17717-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="17717-111">Permission type</span></span>|<span data-ttu-id="17717-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="17717-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17717-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="17717-113">Delegated (work or school account)</span></span>|<span data-ttu-id="17717-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="17717-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="17717-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="17717-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17717-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17717-116">Not supported.</span></span>|
|<span data-ttu-id="17717-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="17717-117">Application</span></span>|<span data-ttu-id="17717-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="17717-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17717-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="17717-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/rootCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17717-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="17717-120">Optional query parameters</span></span>
<span data-ttu-id="17717-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="17717-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="17717-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="17717-122">Request headers</span></span>
|<span data-ttu-id="17717-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="17717-123">Header</span></span>|<span data-ttu-id="17717-124">Wert</span><span class="sxs-lookup"><span data-stu-id="17717-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17717-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="17717-125">Authorization</span></span>|<span data-ttu-id="17717-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="17717-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17717-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="17717-127">Accept</span></span>|<span data-ttu-id="17717-128">application/json</span><span class="sxs-lookup"><span data-stu-id="17717-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17717-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="17717-129">Request body</span></span>
<span data-ttu-id="17717-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="17717-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17717-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="17717-131">Response</span></span>
<span data-ttu-id="17717-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="17717-132">If successful, this method returns a `200 OK` response code and [windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17717-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="17717-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="17717-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="17717-134">Request</span></span>
<span data-ttu-id="17717-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="17717-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}
```

### <a name="response"></a><span data-ttu-id="17717-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="17717-136">Response</span></span>
<span data-ttu-id="17717-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="17717-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 644

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81TrustedRootCertificate",
    "id": "3fb588f9-88f9-3fb5-f988-b53ff988b53f",
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
    "certFileName": "Cert File Name value",
    "destinationStore": "computerCertStoreIntermediate"
  }
}
```





