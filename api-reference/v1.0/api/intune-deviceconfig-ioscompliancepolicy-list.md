---
title: Auflisten von „iosCompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosCompliancePolicy auf.
ms.openlocfilehash: 6722a04f6e4c60ba954d5c09d84de5c4ac86f41c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016769"
---
# <a name="list-ioscompliancepolicies"></a><span data-ttu-id="9b568-103">Auflisten von „iosCompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="9b568-103">List iosCompliancePolicies</span></span>

> <span data-ttu-id="9b568-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9b568-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b568-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="9b568-105">List properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9b568-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9b568-106">Prerequisites</span></span>
<span data-ttu-id="9b568-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b568-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9b568-109">Permission type</span></span>|<span data-ttu-id="9b568-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9b568-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b568-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9b568-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9b568-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b568-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9b568-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9b568-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b568-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b568-114">Not supported.</span></span>|
|<span data-ttu-id="9b568-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9b568-115">Application</span></span>|<span data-ttu-id="9b568-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9b568-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b568-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b568-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="9b568-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9b568-118">Request headers</span></span>
|<span data-ttu-id="9b568-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9b568-119">Header</span></span>|<span data-ttu-id="9b568-120">Wert</span><span class="sxs-lookup"><span data-stu-id="9b568-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b568-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b568-121">Authorization</span></span>|<span data-ttu-id="9b568-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9b568-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b568-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9b568-123">Accept</span></span>|<span data-ttu-id="9b568-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9b568-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b568-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9b568-125">Request body</span></span>
<span data-ttu-id="9b568-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9b568-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b568-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b568-127">Response</span></span>
<span data-ttu-id="9b568-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9b568-128">If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b568-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9b568-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9b568-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9b568-130">Request</span></span>
<span data-ttu-id="9b568-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9b568-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="9b568-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9b568-132">Response</span></span>
<span data-ttu-id="9b568-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9b568-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1034

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCompliancePolicy",
      "id": "4f501351-1351-4f50-5113-504f5113504f",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passcodeBlockSimple": true,
      "passcodeExpirationDays": 6,
      "passcodeMinimumLength": 5,
      "passcodeMinutesOfInactivityBeforeLock": 5,
      "passcodePreviousPasscodeBlockCount": 2,
      "passcodeMinimumCharacterSetCount": 0,
      "passcodeRequiredType": "alphanumeric",
      "passcodeRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "securityBlockJailbrokenDevices": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "managedEmailProfileRequired": true
    }
  ]
}
```



