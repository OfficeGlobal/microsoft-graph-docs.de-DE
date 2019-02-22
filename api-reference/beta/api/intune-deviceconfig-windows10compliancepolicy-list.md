---
title: Auflisten von „windows10CompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windows10CompliancePolicy auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b00291d66849c579c7e7760a7c541477c934c617
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158338"
---
# <a name="list-windows10compliancepolicies"></a><span data-ttu-id="84207-103">Auflisten von „windows10CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="84207-103">List windows10CompliancePolicies</span></span>

> <span data-ttu-id="84207-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84207-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84207-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="84207-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84207-106">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="84207-106">List properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84207-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="84207-107">Prerequisites</span></span>
<span data-ttu-id="84207-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="84207-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="84207-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84207-110">Permission type</span></span>|<span data-ttu-id="84207-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84207-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84207-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84207-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84207-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="84207-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="84207-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84207-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84207-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84207-115">Not supported.</span></span>|
|<span data-ttu-id="84207-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84207-116">Application</span></span>|<span data-ttu-id="84207-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84207-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84207-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84207-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="84207-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84207-119">Request headers</span></span>
|<span data-ttu-id="84207-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="84207-120">Header</span></span>|<span data-ttu-id="84207-121">Wert</span><span class="sxs-lookup"><span data-stu-id="84207-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84207-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84207-122">Authorization</span></span>|<span data-ttu-id="84207-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="84207-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84207-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="84207-124">Accept</span></span>|<span data-ttu-id="84207-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84207-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84207-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="84207-126">Request body</span></span>
<span data-ttu-id="84207-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="84207-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84207-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="84207-128">Response</span></span>
<span data-ttu-id="84207-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="84207-129">If successful, this method returns a `200 OK` response code and a collection of [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84207-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84207-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="84207-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84207-131">Request</span></span>
<span data-ttu-id="84207-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84207-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="84207-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="84207-133">Response</span></span>
<span data-ttu-id="84207-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84207-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2059

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "2919ae62-ae62-2919-62ae-192962ae1929",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordRequiredToUnlockFromIdle": true,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "requireHealthyDeviceReport": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
      "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
      "earlyLaunchAntiMalwareDriverEnabled": true,
      "bitLockerEnabled": true,
      "secureBootEnabled": true,
      "codeIntegrityEnabled": true,
      "storageRequireEncryption": true,
      "activeFirewallRequired": true,
      "defenderEnabled": true,
      "defenderVersion": "Defender Version value",
      "signatureOutOfDate": true,
      "rtpEnabled": true,
      "antivirusRequired": true,
      "antiSpywareRequired": true,
      "validOperatingSystemBuildRanges": [
        {
          "@odata.type": "microsoft.graph.operatingSystemVersionRange",
          "description": "Description value",
          "lowestVersion": "Lowest Version value",
          "highestVersion": "Highest Version value"
        }
      ],
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "configurationManagerComplianceRequired": true
    }
  ]
}
```




