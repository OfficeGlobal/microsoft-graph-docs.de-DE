---
title: Abrufen von „iosManagedAppProtection“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs iosManagedAppProtection.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3c799fdb0c726a2d4803e853b1cdd97e02e1119
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973103"
---
# <a name="get-iosmanagedappprotection"></a><span data-ttu-id="c8ec4-103">Abrufen von „iosManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="c8ec4-103">Get iosManagedAppProtection</span></span>

> <span data-ttu-id="c8ec4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8ec4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8ec4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c8ec4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8ec4-106">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span><span class="sxs-lookup"><span data-stu-id="c8ec4-106">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8ec4-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c8ec4-107">Prerequisites</span></span>
<span data-ttu-id="c8ec4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8ec4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8ec4-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8ec4-110">Permission type</span></span>|<span data-ttu-id="c8ec4-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8ec4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8ec4-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8ec4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8ec4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8ec4-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c8ec4-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8ec4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8ec4-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8ec4-115">Not supported.</span></span>|
|<span data-ttu-id="c8ec4-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8ec4-116">Application</span></span>|<span data-ttu-id="c8ec4-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8ec4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8ec4-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8ec4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8ec4-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c8ec4-119">Optional query parameters</span></span>
<span data-ttu-id="c8ec4-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c8ec4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8ec4-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8ec4-121">Request headers</span></span>
|<span data-ttu-id="c8ec4-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c8ec4-122">Header</span></span>|<span data-ttu-id="c8ec4-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c8ec4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8ec4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8ec4-124">Authorization</span></span>|<span data-ttu-id="c8ec4-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c8ec4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8ec4-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c8ec4-126">Accept</span></span>|<span data-ttu-id="c8ec4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c8ec4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8ec4-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8ec4-128">Request body</span></span>
<span data-ttu-id="c8ec4-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c8ec4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8ec4-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8ec4-130">Response</span></span>
<span data-ttu-id="c8ec4-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c8ec4-131">If successful, this method returns a `200 OK` response code and [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8ec4-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8ec4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8ec4-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8ec4-133">Request</span></span>
<span data-ttu-id="c8ec4-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8ec4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}
```

### <a name="response"></a><span data-ttu-id="c8ec4-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8ec4-135">Response</span></span>
<span data-ttu-id="c8ec4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8ec4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2863

{
  "value": {
    "@odata.type": "#microsoft.graph.iosManagedAppProtection",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
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
    "allowedOutboundClipboardSharingExceptionLength": 14,
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




