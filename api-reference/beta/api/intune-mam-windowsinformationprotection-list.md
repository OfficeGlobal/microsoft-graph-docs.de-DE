---
title: Auflisten von „windowsInformationProtection“
description: Listet die Eigenschaften und Beziehungen der windowsInformationProtection-Objekte auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9f8e50e3ebcce6d45242f8f49fd120a892f54161
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399402"
---
# <a name="list-windowsinformationprotections"></a><span data-ttu-id="48042-103">Auflisten von „windowsInformationProtection“</span><span class="sxs-lookup"><span data-stu-id="48042-103">List windowsInformationProtections</span></span>

> <span data-ttu-id="48042-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="48042-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="48042-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="48042-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="48042-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="48042-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48042-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="48042-107">List properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="48042-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="48042-108">Prerequisites</span></span>
<span data-ttu-id="48042-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="48042-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="48042-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="48042-111">Permission type</span></span>|<span data-ttu-id="48042-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="48042-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48042-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="48042-113">Delegated (work or school account)</span></span>|<span data-ttu-id="48042-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="48042-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="48042-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="48042-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48042-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48042-116">Not supported.</span></span>|
|<span data-ttu-id="48042-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="48042-117">Application</span></span>|<span data-ttu-id="48042-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="48042-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48042-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="48042-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="48042-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="48042-120">Request headers</span></span>
|<span data-ttu-id="48042-121">Header</span><span class="sxs-lookup"><span data-stu-id="48042-121">Header</span></span>|<span data-ttu-id="48042-122">Wert</span><span class="sxs-lookup"><span data-stu-id="48042-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48042-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="48042-123">Authorization</span></span>|<span data-ttu-id="48042-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="48042-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="48042-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="48042-125">Accept</span></span>|<span data-ttu-id="48042-126">application/json</span><span class="sxs-lookup"><span data-stu-id="48042-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48042-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="48042-127">Request body</span></span>
<span data-ttu-id="48042-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="48042-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48042-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="48042-129">Response</span></span>
<span data-ttu-id="48042-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="48042-130">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48042-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="48042-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="48042-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="48042-132">Request</span></span>
<span data-ttu-id="48042-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="48042-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="48042-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="48042-134">Response</span></span>
<span data-ttu-id="48042-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="48042-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4675

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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




