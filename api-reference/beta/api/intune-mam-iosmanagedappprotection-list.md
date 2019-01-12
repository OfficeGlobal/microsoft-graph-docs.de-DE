---
title: Auflisten von „iosManagedAppProtection“
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs iosManagedAppProtection auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9dee560632b3da520537ad9f59b05d02e966cc98
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930950"
---
# <a name="list-iosmanagedappprotections"></a><span data-ttu-id="975d6-103">Auflisten von „iosManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="975d6-103">List iosManagedAppProtections</span></span>

> <span data-ttu-id="975d6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="975d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="975d6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="975d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="975d6-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="975d6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="975d6-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="975d6-107">List properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="975d6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="975d6-108">Prerequisites</span></span>
<span data-ttu-id="975d6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="975d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="975d6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="975d6-111">Permission type</span></span>|<span data-ttu-id="975d6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="975d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="975d6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="975d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="975d6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="975d6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="975d6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="975d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="975d6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="975d6-116">Not supported.</span></span>|
|<span data-ttu-id="975d6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="975d6-117">Application</span></span>|<span data-ttu-id="975d6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="975d6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="975d6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="975d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="975d6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="975d6-120">Request headers</span></span>
|<span data-ttu-id="975d6-121">Header</span><span class="sxs-lookup"><span data-stu-id="975d6-121">Header</span></span>|<span data-ttu-id="975d6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="975d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="975d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="975d6-123">Authorization</span></span>|<span data-ttu-id="975d6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="975d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="975d6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="975d6-125">Accept</span></span>|<span data-ttu-id="975d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="975d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="975d6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="975d6-127">Request body</span></span>
<span data-ttu-id="975d6-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="975d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="975d6-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="975d6-129">Response</span></span>
<span data-ttu-id="975d6-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="975d6-130">If successful, this method returns a `200 OK` response code and a collection of [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="975d6-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="975d6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="975d6-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="975d6-132">Request</span></span>
<span data-ttu-id="975d6-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="975d6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="975d6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="975d6-134">Response</span></span>
<span data-ttu-id="975d6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="975d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2870

{
  "value": [
    {
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
  ]
}
```





