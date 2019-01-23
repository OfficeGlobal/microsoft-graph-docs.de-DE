---
title: Auflisten von „windows10CompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windows10CompliancePolicy auf.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4143f0662ff3299c62c851ccbae2376a0661e133
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393172"
---
# <a name="list-windows10compliancepolicies"></a><span data-ttu-id="ce6d6-103">Auflisten von „windows10CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="ce6d6-103">List windows10CompliancePolicies</span></span>

> <span data-ttu-id="ce6d6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ce6d6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ce6d6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ce6d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce6d6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ce6d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce6d6-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="ce6d6-107">List properties and relationships of the [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce6d6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ce6d6-108">Prerequisites</span></span>
<span data-ttu-id="ce6d6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ce6d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ce6d6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce6d6-111">Permission type</span></span>|<span data-ttu-id="ce6d6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce6d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce6d6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce6d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce6d6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce6d6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ce6d6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce6d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce6d6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce6d6-116">Not supported.</span></span>|
|<span data-ttu-id="ce6d6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce6d6-117">Application</span></span>|<span data-ttu-id="ce6d6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce6d6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce6d6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce6d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="ce6d6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce6d6-120">Request headers</span></span>
|<span data-ttu-id="ce6d6-121">Header</span><span class="sxs-lookup"><span data-stu-id="ce6d6-121">Header</span></span>|<span data-ttu-id="ce6d6-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ce6d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce6d6-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="ce6d6-123">Authorization</span></span>|<span data-ttu-id="ce6d6-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ce6d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce6d6-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ce6d6-125">Accept</span></span>|<span data-ttu-id="ce6d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce6d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce6d6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce6d6-127">Request body</span></span>
<span data-ttu-id="ce6d6-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ce6d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce6d6-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce6d6-129">Response</span></span>
<span data-ttu-id="ce6d6-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ce6d6-130">If successful, this method returns a `200 OK` response code and a collection of [windows10CompliancePolicy](../resources/intune-deviceconfig-windows10compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce6d6-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce6d6-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce6d6-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce6d6-132">Request</span></span>
<span data-ttu-id="ce6d6-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ce6d6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="ce6d6-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce6d6-134">Response</span></span>
<span data-ttu-id="ce6d6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce6d6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




