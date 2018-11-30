---
title: Abrufen von „iosManagedAppProtection“
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs iosManagedAppProtection.
ms.openlocfilehash: 2dd50cbc226b7a5c0888d14eeb0f20c3502f2378
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060460"
---
# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="3b473-103">Abrufen von „iosManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="3b473-103">Get iosManagedAppProtection</span></span>

> <span data-ttu-id="3b473-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b473-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b473-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b473-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b473-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3b473-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b473-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="3b473-107">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b473-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3b473-108">Prerequisites</span></span>
<span data-ttu-id="3b473-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b473-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b473-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b473-111">Permission type</span></span>|<span data-ttu-id="3b473-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b473-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b473-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b473-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b473-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b473-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3b473-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b473-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b473-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b473-116">Not supported.</span></span>|
|<span data-ttu-id="3b473-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b473-117">Application</span></span>|<span data-ttu-id="3b473-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b473-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b473-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b473-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b473-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3b473-120">Optional query parameters</span></span>
<span data-ttu-id="3b473-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3b473-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3b473-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b473-122">Request headers</span></span>
|<span data-ttu-id="3b473-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3b473-123">Header</span></span>|<span data-ttu-id="3b473-124">Wert</span><span class="sxs-lookup"><span data-stu-id="3b473-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b473-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b473-125">Authorization</span></span>|<span data-ttu-id="3b473-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3b473-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b473-127">Accept</span><span class="sxs-lookup"><span data-stu-id="3b473-127">Accept</span></span>|<span data-ttu-id="3b473-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3b473-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b473-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b473-129">Request body</span></span>
<span data-ttu-id="3b473-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3b473-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b473-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b473-131">Response</span></span>
<span data-ttu-id="3b473-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3b473-132">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b473-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b473-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b473-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b473-134">Request</span></span>
<span data-ttu-id="3b473-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b473-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="3b473-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b473-136">Response</span></span>
<span data-ttu-id="3b473-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b473-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2736

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
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
    "minimumWipeOsVersion": "Minimum Wipe Os Version value",
    "minimumWipeAppVersion": "Minimum Wipe App Version value",
    "appActionIfDeviceComplianceRequired": "wipe",
    "appActionIfMaximumPinRetriesExceeded": "wipe",
    "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
    "isAssigned": true,
    "targetedAppManagementLevels": "unmanaged",
    "appDataEncryptionType": "afterDeviceRestart",
    "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
    "deployedAppCount": 0,
    "faceIdBlocked": true,
    "exemptedAppProtocols": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ],
    "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
    "allowedIosDeviceModels": "Allowed Ios Device Models value",
    "appActionIfIosDeviceModelNotAllowed": "wipe",
    "thirdPartyKeyboardsBlocked": true,
    "filterOpenInToOnlyManagedApps": true,
    "disableProtectionOfManagedOutboundOpenInData": true,
    "protectInboundDataFromUnknownSources": true
  }
}
```





