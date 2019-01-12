---
title: Auflisten von „macOSCompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs macOSCompliancePolicy auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4432ee81a04b85165f188d0f4fd20e8ec6ac2271
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954260"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="90080-103">Auflisten von „macOSCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="90080-103">List macOSCompliancePolicies</span></span>

> <span data-ttu-id="90080-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="90080-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90080-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="90080-105">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="90080-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="90080-106">Prerequisites</span></span>
<span data-ttu-id="90080-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90080-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90080-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="90080-109">Permission type</span></span>|<span data-ttu-id="90080-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="90080-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90080-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="90080-111">Delegated (work or school account)</span></span>|<span data-ttu-id="90080-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90080-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="90080-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="90080-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90080-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90080-114">Not supported.</span></span>|
|<span data-ttu-id="90080-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="90080-115">Application</span></span>|<span data-ttu-id="90080-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90080-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90080-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="90080-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="90080-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="90080-118">Request headers</span></span>
|<span data-ttu-id="90080-119">Header</span><span class="sxs-lookup"><span data-stu-id="90080-119">Header</span></span>|<span data-ttu-id="90080-120">Wert</span><span class="sxs-lookup"><span data-stu-id="90080-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90080-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="90080-121">Authorization</span></span>|<span data-ttu-id="90080-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="90080-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90080-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="90080-123">Accept</span></span>|<span data-ttu-id="90080-124">application/json</span><span class="sxs-lookup"><span data-stu-id="90080-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90080-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="90080-125">Request body</span></span>
<span data-ttu-id="90080-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="90080-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90080-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="90080-127">Response</span></span>
<span data-ttu-id="90080-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="90080-128">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90080-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="90080-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="90080-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="90080-130">Request</span></span>
<span data-ttu-id="90080-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="90080-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="90080-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="90080-132">Response</span></span>
<span data-ttu-id="90080-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90080-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1150

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
      "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "systemIntegrityProtectionEnabled": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "storageRequireEncryption": true,
      "firewallEnabled": true,
      "firewallBlockAllIncoming": true,
      "firewallEnableStealthMode": true
    }
  ]
}
```



