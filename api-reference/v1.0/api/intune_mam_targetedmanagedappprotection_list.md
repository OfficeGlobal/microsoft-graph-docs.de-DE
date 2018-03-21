# <a name="list-targetedmanagedappprotections"></a><span data-ttu-id="bc3ed-101">targetedManagedAppProtections auflisten</span><span class="sxs-lookup"><span data-stu-id="bc3ed-101">List targetedManagedAppProtections</span></span>

> <span data-ttu-id="bc3ed-102">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bc3ed-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc3ed-103">Listet die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="bc3ed-103">List properties and relationships of the [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc3ed-104">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bc3ed-104">Prerequisites</span></span>
<span data-ttu-id="bc3ed-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc3ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bc3ed-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc3ed-107">Permission type</span></span>|<span data-ttu-id="bc3ed-108">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc3ed-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc3ed-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc3ed-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bc3ed-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc3ed-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bc3ed-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc3ed-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc3ed-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc3ed-112">Not supported.</span></span>|
|<span data-ttu-id="bc3ed-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc3ed-113">Application</span></span>|<span data-ttu-id="bc3ed-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc3ed-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc3ed-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc3ed-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="bc3ed-116">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc3ed-116">Request headers</span></span>
|<span data-ttu-id="bc3ed-117">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bc3ed-117">Header</span></span>|<span data-ttu-id="bc3ed-118">Wert</span><span class="sxs-lookup"><span data-stu-id="bc3ed-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc3ed-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc3ed-119">Authorization</span></span>|<span data-ttu-id="bc3ed-120">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc3ed-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bc3ed-121">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bc3ed-121">Accept</span></span>|<span data-ttu-id="bc3ed-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bc3ed-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc3ed-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc3ed-123">Request body</span></span>
<span data-ttu-id="bc3ed-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bc3ed-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc3ed-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc3ed-125">Response</span></span>
<span data-ttu-id="bc3ed-126">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc3ed-126">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/intune_mam_targetedmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc3ed-127">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc3ed-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc3ed-128">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc3ed-128">Request</span></span>
<span data-ttu-id="bc3ed-129">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc3ed-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="bc3ed-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc3ed-130">Response</span></span>
<span data-ttu-id="bc3ed-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc3ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1750

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "b6b92266-2266-b6b9-6622-b9b66622b9b6",
      "version": "Version value",
      "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
      "periodOnlineBeforeAccessCheck": "PT35.0018757S",
      "allowedInboundDataTransferSources": "managedApps",
      "allowedOutboundDataTransferDestinations": "managedApps",
      "organizationalCredentialsRequired": true,
      "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
      "dataBackupBlocked": true,
      "deviceComplianceRequired": true,
      "managedBrowserToOpenLinksRequired": true,
      "saveAsBlocked": true,
      "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
      "pinRequired": true,
      "maximumPinRetries": 1,
      "simplePinBlocked": true,
      "minimumPinLength": 0,
      "pinCharacterSet": "alphanumericAndSymbol",
      "periodBeforePinReset": "PT3M29.6631862S",
      "allowedDataStorageLocations": [
        "sharePoint"
      ],
      "contactSyncBlocked": true,
      "printBlocked": true,
      "fingerprintBlocked": true,
      "disableAppPinIfDevicePinIsSet": true,
      "minimumRequiredOsVersion": "Minimum Required Os Version value",
      "minimumWarningOsVersion": "Minimum Warning Os Version value",
      "minimumRequiredAppVersion": "Minimum Required App Version value",
      "minimumWarningAppVersion": "Minimum Warning App Version value",
      "isAssigned": true
    }
  ]
}
```



