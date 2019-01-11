---
title: Auflisten von „managedAppProtection“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs managedAppProtection auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a7faca1fe1d84d5b4ac73cc63e1ed694c50358f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867998"
---
# <a name="list-managedappprotections"></a><span data-ttu-id="fea9d-103">Auflisten von „managedAppProtection“</span><span class="sxs-lookup"><span data-stu-id="fea9d-103">List managedAppProtections</span></span>

> <span data-ttu-id="fea9d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fea9d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fea9d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fea9d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fea9d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fea9d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fea9d-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md) auf.</span><span class="sxs-lookup"><span data-stu-id="fea9d-107">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fea9d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fea9d-108">Prerequisites</span></span>
<span data-ttu-id="fea9d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fea9d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fea9d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fea9d-111">Permission type</span></span>|<span data-ttu-id="fea9d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fea9d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fea9d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fea9d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fea9d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fea9d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fea9d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fea9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fea9d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fea9d-116">Not supported.</span></span>|
|<span data-ttu-id="fea9d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fea9d-117">Application</span></span>|<span data-ttu-id="fea9d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fea9d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fea9d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fea9d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="fea9d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fea9d-120">Request headers</span></span>
|<span data-ttu-id="fea9d-121">Header</span><span class="sxs-lookup"><span data-stu-id="fea9d-121">Header</span></span>|<span data-ttu-id="fea9d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fea9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fea9d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fea9d-123">Authorization</span></span>|<span data-ttu-id="fea9d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fea9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fea9d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fea9d-125">Accept</span></span>|<span data-ttu-id="fea9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fea9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fea9d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fea9d-127">Request body</span></span>
<span data-ttu-id="fea9d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fea9d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fea9d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="fea9d-129">Response</span></span>
<span data-ttu-id="fea9d-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [managedAppProtection](../resources/intune-mam-managedappprotection.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fea9d-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fea9d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fea9d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fea9d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fea9d-132">Request</span></span>
<span data-ttu-id="fea9d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fea9d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="fea9d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fea9d-134">Response</span></span>
<span data-ttu-id="fea9d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fea9d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2020

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppProtection",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "a6c064ce-64ce-a6c0-ce64-c0a6ce64c0a6",
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
      "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S"
    }
  ]
}
```





