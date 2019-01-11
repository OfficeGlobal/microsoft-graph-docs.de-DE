---
title: Auflisten von „windowsInformationProtection“
description: Listet die Eigenschaften und Beziehungen der windowsInformationProtection-Objekte auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dc8b9245bf71b8c7c81ea3a51e260ff3bca557da
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889831"
---
# <a name="list-windowsinformationprotections"></a><span data-ttu-id="da258-103">Auflisten von „windowsInformationProtection“</span><span class="sxs-lookup"><span data-stu-id="da258-103">List windowsInformationProtections</span></span>

> <span data-ttu-id="da258-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="da258-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da258-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="da258-105">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da258-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="da258-106">Prerequisites</span></span>
<span data-ttu-id="da258-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da258-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da258-109">Permission type</span></span>|<span data-ttu-id="da258-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da258-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da258-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da258-111">Delegated (work or school account)</span></span>|<span data-ttu-id="da258-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="da258-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="da258-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da258-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da258-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da258-114">Not supported.</span></span>|
|<span data-ttu-id="da258-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da258-115">Application</span></span>|<span data-ttu-id="da258-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da258-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da258-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da258-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="da258-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da258-118">Request headers</span></span>
|<span data-ttu-id="da258-119">Header</span><span class="sxs-lookup"><span data-stu-id="da258-119">Header</span></span>|<span data-ttu-id="da258-120">Wert</span><span class="sxs-lookup"><span data-stu-id="da258-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da258-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="da258-121">Authorization</span></span>|<span data-ttu-id="da258-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="da258-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da258-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="da258-123">Accept</span></span>|<span data-ttu-id="da258-124">application/json</span><span class="sxs-lookup"><span data-stu-id="da258-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da258-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da258-125">Request body</span></span>
<span data-ttu-id="da258-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="da258-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da258-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="da258-127">Response</span></span>
<span data-ttu-id="da258-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="da258-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da258-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da258-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="da258-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da258-130">Request</span></span>
<span data-ttu-id="da258-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da258-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="da258-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="da258-132">Response</span></span>
<span data-ttu-id="da258-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da258-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4601

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "ca339419-9419-ca33-1994-33ca199433ca",
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



