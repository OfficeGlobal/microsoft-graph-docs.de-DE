---
title: Auflisten von „windows10MobileCompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windows10MobileCompliancePolicy auf.
ms.openlocfilehash: d2e0e17f3112be1ba90a99e2d94edc96b25a74fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016376"
---
# <a name="list-windows10mobilecompliancepolicies"></a><span data-ttu-id="97939-103">Auflisten von „windows10MobileCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="97939-103">List windows10MobileCompliancePolicies</span></span>

> <span data-ttu-id="97939-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="97939-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97939-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="97939-105">List properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97939-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="97939-106">Prerequisites</span></span>
<span data-ttu-id="97939-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97939-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97939-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97939-109">Permission type</span></span>|<span data-ttu-id="97939-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97939-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97939-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97939-111">Delegated (work or school account)</span></span>|<span data-ttu-id="97939-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97939-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="97939-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97939-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97939-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97939-114">Not supported.</span></span>|
|<span data-ttu-id="97939-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97939-115">Application</span></span>|<span data-ttu-id="97939-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97939-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97939-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97939-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="97939-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97939-118">Request headers</span></span>
|<span data-ttu-id="97939-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="97939-119">Header</span></span>|<span data-ttu-id="97939-120">Wert</span><span class="sxs-lookup"><span data-stu-id="97939-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97939-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="97939-121">Authorization</span></span>|<span data-ttu-id="97939-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="97939-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97939-123">Accept</span><span class="sxs-lookup"><span data-stu-id="97939-123">Accept</span></span>|<span data-ttu-id="97939-124">application/json</span><span class="sxs-lookup"><span data-stu-id="97939-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97939-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97939-125">Request body</span></span>
<span data-ttu-id="97939-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="97939-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97939-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="97939-127">Response</span></span>
<span data-ttu-id="97939-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="97939-128">If successful, this method returns a `200 OK` response code and a collection of [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97939-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97939-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="97939-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97939-130">Request</span></span>
<span data-ttu-id="97939-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97939-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="97939-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="97939-132">Response</span></span>
<span data-ttu-id="97939-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97939-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1089

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
      "id": "3d4237b0-37b0-3d42-b037-423db037423d",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordMinimumLength": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "passwordExpirationDays": 6,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordRequireToUnlockFromIdle": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "earlyLaunchAntiMalwareDriverEnabled": true,
      "bitLockerEnabled": true,
      "secureBootEnabled": true,
      "codeIntegrityEnabled": true,
      "storageRequireEncryption": true
    }
  ]
}
```



