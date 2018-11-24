# <a name="get-windowsinformationprotection"></a><span data-ttu-id="fd042-101">windowsInformationProtection abrufen</span><span class="sxs-lookup"><span data-stu-id="fd042-101">Get windowsInformationProtection</span></span>

> <span data-ttu-id="fd042-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fd042-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd042-103">Liest die Eigenschaften und Beziehungen des [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)-Objekts auf.</span><span class="sxs-lookup"><span data-stu-id="fd042-103">Read properties and relationships of the [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd042-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fd042-104">Prerequisites</span></span>
<span data-ttu-id="fd042-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fd042-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fd042-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd042-107">Permission type</span></span>|<span data-ttu-id="fd042-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd042-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd042-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd042-109">Delegated (work or school account)</span></span>|<span data-ttu-id="fd042-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd042-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fd042-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd042-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd042-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd042-112">Not supported.</span></span>|
|<span data-ttu-id="fd042-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd042-113">Application</span></span>|<span data-ttu-id="fd042-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd042-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd042-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd042-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd042-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fd042-116">Optional query parameters</span></span>
<span data-ttu-id="fd042-117">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd042-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fd042-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd042-118">Request headers</span></span>
|<span data-ttu-id="fd042-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fd042-119">Header</span></span>|<span data-ttu-id="fd042-120">Wert</span><span class="sxs-lookup"><span data-stu-id="fd042-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd042-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd042-121">Authorization</span></span>|<span data-ttu-id="fd042-122">Bearer &lt;token&gt;. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd042-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd042-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fd042-123">Accept</span></span>|<span data-ttu-id="fd042-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fd042-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd042-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd042-125">Request body</span></span>
<span data-ttu-id="fd042-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fd042-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd042-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd042-127">Response</span></span>
<span data-ttu-id="fd042-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd042-128">If successful, this method returns a `200 OK` response code and [windowsInformationProtection](../resources/intune_mam_windowsinformationprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd042-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd042-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd042-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd042-130">Request</span></span>
<span data-ttu-id="fd042-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd042-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="fd042-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd042-132">Response</span></span>
<span data-ttu-id="fd042-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd042-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4337

{
  "value": {
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
}
```



