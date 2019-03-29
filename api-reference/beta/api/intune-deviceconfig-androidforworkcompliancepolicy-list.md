---
title: AndroidForWorkCompliancePolicies aufListen
description: AufListen von Eigenschaften und Beziehungen der androidForWorkCompliancePolicy-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61318e2638d5711a5879d79746db978931bf36d2
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980726"
---
# <a name="list-androidforworkcompliancepolicies"></a><span data-ttu-id="3b142-103">AndroidForWorkCompliancePolicies aufListen</span><span class="sxs-lookup"><span data-stu-id="3b142-103">List androidForWorkCompliancePolicies</span></span>

> <span data-ttu-id="3b142-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b142-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b142-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3b142-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b142-106">AufListen von Eigenschaften und Beziehungen der [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="3b142-106">List properties and relationships of the [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b142-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3b142-107">Prerequisites</span></span>
<span data-ttu-id="3b142-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b142-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b142-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b142-110">Permission type</span></span>|<span data-ttu-id="3b142-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b142-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b142-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b142-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b142-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3b142-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3b142-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b142-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b142-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b142-115">Not supported.</span></span>|
|<span data-ttu-id="3b142-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b142-116">Application</span></span>|<span data-ttu-id="3b142-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b142-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b142-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b142-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3b142-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b142-119">Request headers</span></span>
|<span data-ttu-id="3b142-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3b142-120">Header</span></span>|<span data-ttu-id="3b142-121">Wert</span><span class="sxs-lookup"><span data-stu-id="3b142-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b142-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b142-122">Authorization</span></span>|<span data-ttu-id="3b142-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3b142-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b142-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3b142-124">Accept</span></span>|<span data-ttu-id="3b142-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b142-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b142-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b142-126">Request body</span></span>
<span data-ttu-id="3b142-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3b142-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b142-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b142-128">Response</span></span>
<span data-ttu-id="3b142-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3b142-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkCompliancePolicy](../resources/intune-deviceconfig-androidforworkcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b142-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b142-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b142-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b142-131">Request</span></span>
<span data-ttu-id="3b142-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b142-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="3b142-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b142-133">Response</span></span>
<span data-ttu-id="3b142-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b142-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1616

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "a8d667bd-67bd-a8d6-bd67-d6a8bd67d6a8",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordMinimumLength": 5,
      "passwordRequiredType": "alphabetic",
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "securityPreventInstallAppsFromUnknownSources": true,
      "securityDisableUsbDebugging": true,
      "securityRequireVerifyApps": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "securityBlockJailbrokenDevices": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
      "storageRequireEncryption": true,
      "securityRequireSafetyNetAttestationBasicIntegrity": true,
      "securityRequireSafetyNetAttestationCertifiedDevice": true,
      "securityRequireGooglePlayServices": true,
      "securityRequireUpToDateSecurityProviders": true,
      "securityRequireCompanyPortalAppIntegrity": true
    }
  ]
}
```




