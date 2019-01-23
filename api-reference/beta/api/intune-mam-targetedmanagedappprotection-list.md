---
title: targetedManagedAppProtections auflisten
description: Listet die Eigenschaften und Beziehungen von Objekten des Typs targetedManagedAppProtection auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d266d7648cd584ebe37d1857a823da4824e56569
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411435"
---
# <a name="list-targetedmanagedappprotections"></a><span data-ttu-id="f1f87-103">targetedManagedAppProtections auflisten</span><span class="sxs-lookup"><span data-stu-id="f1f87-103">List targetedManagedAppProtections</span></span>

> <span data-ttu-id="f1f87-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f1f87-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f1f87-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f1f87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1f87-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f1f87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1f87-107">Listet die Eigenschaften und Beziehungen von Objekten des Typs [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="f1f87-107">List properties and relationships of the [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1f87-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="f1f87-108">Prerequisites</span></span>
<span data-ttu-id="f1f87-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f1f87-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f1f87-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f1f87-111">Permission type</span></span>|<span data-ttu-id="f1f87-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f1f87-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1f87-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f1f87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1f87-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f1f87-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f1f87-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f1f87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1f87-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1f87-116">Not supported.</span></span>|
|<span data-ttu-id="f1f87-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f1f87-117">Application</span></span>|<span data-ttu-id="f1f87-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f1f87-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1f87-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1f87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f1f87-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f1f87-120">Request headers</span></span>
|<span data-ttu-id="f1f87-121">Header</span><span class="sxs-lookup"><span data-stu-id="f1f87-121">Header</span></span>|<span data-ttu-id="f1f87-122">Wert</span><span class="sxs-lookup"><span data-stu-id="f1f87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1f87-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="f1f87-123">Authorization</span></span>|<span data-ttu-id="f1f87-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="f1f87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1f87-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="f1f87-125">Accept</span></span>|<span data-ttu-id="f1f87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1f87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1f87-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f1f87-127">Request body</span></span>
<span data-ttu-id="f1f87-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f1f87-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1f87-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1f87-129">Response</span></span>
<span data-ttu-id="f1f87-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1f87-130">If successful, this method returns a `200 OK` response code and a collection of [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1f87-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f1f87-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1f87-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f1f87-132">Request</span></span>
<span data-ttu-id="f1f87-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f1f87-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="f1f87-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f1f87-134">Response</span></span>
<span data-ttu-id="f1f87-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f1f87-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2180

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.targetedManagedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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
      "minimumWipeOsVersion": "Minimum Wipe Os Version value",
      "minimumWipeAppVersion": "Minimum Wipe App Version value",
      "appActionIfDeviceComplianceRequired": "wipe",
      "appActionIfMaximumPinRetriesExceeded": "wipe",
      "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
      "isAssigned": true,
      "targetedAppManagementLevels": "unmanaged"
    }
  ]
}
```




