---
title: windows10CompliancePolicy abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs windows10CompliancePolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e85fb5912f6ae18c8e150a24a5c71157ac4e7b63
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158009"
---
# <a name="get-windows10compliancepolicy"></a><span data-ttu-id="a14cb-103">windows10CompliancePolicy abrufen</span><span class="sxs-lookup"><span data-stu-id="a14cb-103">Get windows10CompliancePolicy</span></span>

> <span data-ttu-id="a14cb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a14cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a14cb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a14cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a14cb-106">Liest die Eigenschaften und Beziehungen von Objekten des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a14cb-106">Read properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a14cb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a14cb-107">Prerequisites</span></span>
<span data-ttu-id="a14cb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a14cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a14cb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a14cb-110">Permission type</span></span>|<span data-ttu-id="a14cb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a14cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a14cb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a14cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a14cb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a14cb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a14cb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a14cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a14cb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a14cb-115">Not supported.</span></span>|
|<span data-ttu-id="a14cb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a14cb-116">Application</span></span>|<span data-ttu-id="a14cb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a14cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a14cb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a14cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a14cb-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a14cb-119">Optional query parameters</span></span>
<span data-ttu-id="a14cb-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a14cb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a14cb-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a14cb-121">Request headers</span></span>
|<span data-ttu-id="a14cb-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="a14cb-122">Header</span></span>|<span data-ttu-id="a14cb-123">Wert</span><span class="sxs-lookup"><span data-stu-id="a14cb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a14cb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a14cb-124">Authorization</span></span>|<span data-ttu-id="a14cb-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a14cb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a14cb-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a14cb-126">Accept</span></span>|<span data-ttu-id="a14cb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a14cb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a14cb-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a14cb-128">Request body</span></span>
<span data-ttu-id="a14cb-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a14cb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a14cb-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a14cb-130">Response</span></span>
<span data-ttu-id="a14cb-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a14cb-131">If successful, this method returns a `200 OK` response code and [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a14cb-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a14cb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a14cb-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a14cb-133">Request</span></span>
<span data-ttu-id="a14cb-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a14cb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="a14cb-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a14cb-135">Response</span></span>
<span data-ttu-id="a14cb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a14cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1951

{
  "value": {
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
}
```




