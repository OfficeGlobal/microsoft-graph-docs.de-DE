# <a name="list-mdmwindowsinformationprotectionpolicies"></a><span data-ttu-id="eb4d8-101">Auflisten von „mdmWindowsInformationProtectionPolicy“</span><span class="sxs-lookup"><span data-stu-id="eb4d8-101">List mdmWindowsInformationProtectionPolicies</span></span>

> <span data-ttu-id="eb4d8-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eb4d8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb4d8-103">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="eb4d8-103">List properties and relationships of the [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb4d8-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eb4d8-104">Prerequisites</span></span>
<span data-ttu-id="eb4d8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="eb4d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="eb4d8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb4d8-107">Permission type</span></span>|<span data-ttu-id="eb4d8-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb4d8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb4d8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb4d8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="eb4d8-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb4d8-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="eb4d8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb4d8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb4d8-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb4d8-112">Not supported.</span></span>|
|<span data-ttu-id="eb4d8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb4d8-113">Application</span></span>|<span data-ttu-id="eb4d8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb4d8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb4d8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb4d8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

## <a name="request-headers"></a><span data-ttu-id="eb4d8-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb4d8-116">Request headers</span></span>
|<span data-ttu-id="eb4d8-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eb4d8-117">Header</span></span>|<span data-ttu-id="eb4d8-118">Wert</span><span class="sxs-lookup"><span data-stu-id="eb4d8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb4d8-119">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="eb4d8-119">Authorization</span></span>|<span data-ttu-id="eb4d8-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eb4d8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb4d8-121">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="eb4d8-121">Accept</span></span>|<span data-ttu-id="eb4d8-122">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="eb4d8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb4d8-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb4d8-123">Request body</span></span>
<span data-ttu-id="eb4d8-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eb4d8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb4d8-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb4d8-125">Response</span></span>
<span data-ttu-id="eb4d8-126">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eb4d8-126">If successful, this method returns a `200 OK` response code and a collection of [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb4d8-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb4d8-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb4d8-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb4d8-128">Request</span></span>
<span data-ttu-id="eb4d8-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb4d8-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mdmWindowsInformationProtectionPolicies
```

### <a name="response"></a><span data-ttu-id="eb4d8-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb4d8-130">Response</span></span>
<span data-ttu-id="eb4d8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb4d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4607

{
  "value": [
    {
      "@odata.type": "#microsoft.intune_mam_graph.windowsInformationProtectionPolicy",
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
      "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
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








