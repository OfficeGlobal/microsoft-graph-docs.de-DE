---
title: Auflisten von „androidManagedAppProtection“
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs androidManagedAppProtection auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4e1fc0e76f2693ddb638a5436d265452f8594258
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821969"
---
# <a name="list-androidmanagedappprotections"></a><span data-ttu-id="a3813-103">Auflisten von „androidManagedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="a3813-103">List androidManagedAppProtections</span></span>

> <span data-ttu-id="a3813-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a3813-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3813-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a3813-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3813-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="a3813-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3813-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="a3813-107">List properties and relationships of the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3813-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a3813-108">Prerequisites</span></span>
<span data-ttu-id="a3813-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3813-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3813-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a3813-111">Permission type</span></span>|<span data-ttu-id="a3813-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a3813-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3813-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a3813-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3813-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3813-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a3813-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a3813-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3813-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3813-116">Not supported.</span></span>|
|<span data-ttu-id="a3813-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a3813-117">Application</span></span>|<span data-ttu-id="a3813-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a3813-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3813-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3813-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="a3813-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a3813-120">Request headers</span></span>
|<span data-ttu-id="a3813-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a3813-121">Header</span></span>|<span data-ttu-id="a3813-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a3813-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3813-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3813-123">Authorization</span></span>|<span data-ttu-id="a3813-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a3813-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3813-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a3813-125">Accept</span></span>|<span data-ttu-id="a3813-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3813-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3813-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a3813-127">Request body</span></span>
<span data-ttu-id="a3813-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a3813-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3813-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3813-129">Response</span></span>
<span data-ttu-id="a3813-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="a3813-130">If successful, this method returns a `200 OK` response code and a collection of [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3813-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a3813-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3813-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a3813-132">Request</span></span>
<span data-ttu-id="a3813-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a3813-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/androidManagedAppProtections
```

### <a name="response"></a><span data-ttu-id="a3813-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a3813-134">Response</span></span>
<span data-ttu-id="a3813-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a3813-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2835

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
      "screenCaptureBlocked": true,
      "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
      "encryptAppData": true,
      "deployedAppCount": 0,
      "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
      "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
      "exemptedAppPackages": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
      "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
      "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe"
    }
  ]
}
```





