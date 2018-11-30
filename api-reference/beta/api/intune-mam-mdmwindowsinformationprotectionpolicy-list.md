---
title: Auflisten von „mdmWindowsInformationProtectionPolicy“
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs mdmWindowsInformationProtectionPolicy auf.
ms.openlocfilehash: 0709b2d1ed2466cbcf222d5c0ede808e0c5c8c97
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062199"
---
# <a name="list-mdmwindowsinformationprotectionpolicies"></a><span data-ttu-id="bd356-103">Auflisten von „mdmWindowsInformationProtectionPolicy“</span><span class="sxs-lookup"><span data-stu-id="bd356-103">List mdmWindowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="bd356-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bd356-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd356-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd356-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd356-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bd356-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd356-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="bd356-107">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd356-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bd356-108">Prerequisites</span></span>
<span data-ttu-id="bd356-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd356-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd356-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd356-111">Permission type</span></span>|<span data-ttu-id="bd356-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd356-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd356-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd356-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd356-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd356-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bd356-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd356-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd356-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd356-116">Not supported.</span></span>|
|<span data-ttu-id="bd356-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd356-117">Application</span></span>|<span data-ttu-id="bd356-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd356-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd356-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd356-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="bd356-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd356-120">Request headers</span></span>
|<span data-ttu-id="bd356-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bd356-121">Header</span></span>|<span data-ttu-id="bd356-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bd356-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd356-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd356-123">Authorization</span></span>|<span data-ttu-id="bd356-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bd356-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd356-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bd356-125">Accept</span></span>|<span data-ttu-id="bd356-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd356-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd356-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd356-127">Request body</span></span>
<span data-ttu-id="bd356-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bd356-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd356-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd356-129">Response</span></span>
<span data-ttu-id="bd356-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bd356-130">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd356-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bd356-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd356-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd356-132">Request</span></span>
<span data-ttu-id="bd356-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bd356-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="bd356-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd356-134">Response</span></span>
<span data-ttu-id="bd356-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd356-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4610

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "8efb0c35-0c35-8efb-350c-fb8e350cfb8e",
      "version": "Version value",
      "enforcementLevel": "encryptAndAuditOnly",
      "enterpriseDomain": "Enterprise Domain value",
      "enterpriseProtectedDomainNames": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
          "displayName": "Display Name value",
          "resources": [
            "Resources value"
          ]
        }
      ],
      "protectionUnderLockConfigRequired": true,
      "dataRecoveryCertificate": {
        "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
        "subjectName": "Subject Name value",
        "description": "Description value",
        "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
        "certificate": "Y2VydGlmaWNhdGU="
      },
      "revokeOnUnenrollDisabled": true,
      "rightsManagementServicesTemplateId": "abf7b16f-b16f-abf7-6fb1-f7ab6fb1f7ab",
      "azureRightsManagementServicesAllowed": true,
      "iconsVisible": true,
      "protectedApps": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
          "displayName": "Display Name value",
          "description": "Description value",
          "publisherName": "Publisher Name value",
          "productName": "Product Name value",
          "denied": true
        }
      ],
      "exemptApps": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
          "displayName": "Display Name value",
          "description": "Description value",
          "publisherName": "Publisher Name value",
          "productName": "Product Name value",
          "denied": true
        }
      ],
      "enterpriseNetworkDomainNames": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
          "displayName": "Display Name value",
          "resources": [
            "Resources value"
          ]
        }
      ],
      "enterpriseProxiedDomains": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
          "displayName": "Display Name value",
          "proxiedDomains": [
            {
              "@odata.type": "microsoft.graph.proxiedDomain",
              "ipAddressOrFQDN": "Ip Address Or FQDN value",
              "proxy": "Proxy value"
            }
          ]
        }
      ],
      "enterpriseIPRanges": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
          "displayName": "Display Name value",
          "ranges": [
            {
              "@odata.type": "microsoft.graph.iPv6Range",
              "lowerAddress": "Lower Address value",
              "upperAddress": "Upper Address value"
            }
          ]
        }
      ],
      "enterpriseIPRangesAreAuthoritative": true,
      "enterpriseProxyServers": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
          "displayName": "Display Name value",
          "resources": [
            "Resources value"
          ]
        }
      ],
      "enterpriseInternalProxyServers": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
          "displayName": "Display Name value",
          "resources": [
            "Resources value"
          ]
        }
      ],
      "enterpriseProxyServersAreAuthoritative": true,
      "neutralDomainResources": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
          "displayName": "Display Name value",
          "resources": [
            "Resources value"
          ]
        }
      ],
      "indexingEncryptedStoresOrItemsBlocked": true,
      "smbAutoEncryptedFileExtensions": [
        {
          "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
          "displayName": "Display Name value",
          "resources": [
            "Resources value"
          ]
        }
      ],
      "isAssigned": true
    }
  ]
}
```




