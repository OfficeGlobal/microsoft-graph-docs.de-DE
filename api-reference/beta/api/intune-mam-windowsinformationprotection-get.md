---
title: windowsInformationProtection abrufen
description: Liest die Eigenschaften und Beziehungen des windowsInformationProtection-Objekts auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd7fd86a0023f94c4a50eacc5baab3a0bee28439
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957983"
---
# <a name="get-windowsinformationprotection"></a><span data-ttu-id="f6bd0-103">windowsInformationProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="f6bd0-103">Get windowsInformationProtection</span></span>

> <span data-ttu-id="f6bd0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6bd0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6bd0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f6bd0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6bd0-106">Liest die Eigenschaften und Beziehungen des [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)-Objekts auf.</span><span class="sxs-lookup"><span data-stu-id="f6bd0-106">Read properties and relationships of the [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f6bd0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f6bd0-107">Prerequisites</span></span>
<span data-ttu-id="f6bd0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6bd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6bd0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6bd0-110">Permission type</span></span>|<span data-ttu-id="f6bd0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6bd0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6bd0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6bd0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f6bd0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f6bd0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f6bd0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6bd0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6bd0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6bd0-115">Not supported.</span></span>|
|<span data-ttu-id="f6bd0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6bd0-116">Application</span></span>|<span data-ttu-id="f6bd0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f6bd0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6bd0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6bd0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6bd0-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f6bd0-119">Optional query parameters</span></span>
<span data-ttu-id="f6bd0-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f6bd0-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6bd0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6bd0-121">Request headers</span></span>
|<span data-ttu-id="f6bd0-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f6bd0-122">Header</span></span>|<span data-ttu-id="f6bd0-123">Wert</span><span class="sxs-lookup"><span data-stu-id="f6bd0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6bd0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6bd0-124">Authorization</span></span>|<span data-ttu-id="f6bd0-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f6bd0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6bd0-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f6bd0-126">Accept</span></span>|<span data-ttu-id="f6bd0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f6bd0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6bd0-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6bd0-128">Request body</span></span>
<span data-ttu-id="f6bd0-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f6bd0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6bd0-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6bd0-130">Response</span></span>
<span data-ttu-id="f6bd0-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6bd0-131">If successful, this method returns a `200 OK` response code and [windowsInformationProtection](../resources/intune-mam-windowsinformationprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6bd0-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6bd0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f6bd0-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6bd0-133">Request</span></span>
<span data-ttu-id="f6bd0-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6bd0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="f6bd0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6bd0-135">Response</span></span>
<span data-ttu-id="f6bd0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6bd0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4405

{
  "value": {
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
}
```




