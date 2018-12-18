---
title: Auflisten von „windows81CompliancePolicy“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs windows81CompliancePolicy auf.
author: tfitzmac
ms.openlocfilehash: 72c3416677f56380248a83bbf8dd5b22816ccd2f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335364"
---
# <a name="list-windows81compliancepolicies"></a><span data-ttu-id="90309-103">Auflisten von „windows81CompliancePolicy“</span><span class="sxs-lookup"><span data-stu-id="90309-103">List windows81CompliancePolicies</span></span>

> <span data-ttu-id="90309-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="90309-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90309-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) auf.</span><span class="sxs-lookup"><span data-stu-id="90309-105">List properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="90309-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="90309-106">Prerequisites</span></span>
<span data-ttu-id="90309-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90309-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="90309-109">Permission type</span></span>|<span data-ttu-id="90309-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="90309-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90309-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="90309-111">Delegated (work or school account)</span></span>|<span data-ttu-id="90309-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="90309-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="90309-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="90309-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90309-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90309-114">Not supported.</span></span>|
|<span data-ttu-id="90309-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="90309-115">Application</span></span>|<span data-ttu-id="90309-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="90309-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90309-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="90309-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="90309-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="90309-118">Request headers</span></span>
|<span data-ttu-id="90309-119">Header</span><span class="sxs-lookup"><span data-stu-id="90309-119">Header</span></span>|<span data-ttu-id="90309-120">Wert</span><span class="sxs-lookup"><span data-stu-id="90309-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90309-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="90309-121">Authorization</span></span>|<span data-ttu-id="90309-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="90309-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90309-123">Accept</span><span class="sxs-lookup"><span data-stu-id="90309-123">Accept</span></span>|<span data-ttu-id="90309-124">application/json</span><span class="sxs-lookup"><span data-stu-id="90309-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90309-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="90309-125">Request body</span></span>
<span data-ttu-id="90309-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="90309-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90309-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="90309-127">Response</span></span>
<span data-ttu-id="90309-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="90309-128">If successful, this method returns a `200 OK` response code and a collection of [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90309-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="90309-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="90309-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="90309-130">Request</span></span>
<span data-ttu-id="90309-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="90309-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="90309-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="90309-132">Response</span></span>
<span data-ttu-id="90309-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="90309-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 879

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
      "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
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
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "storageRequireEncryption": true
    }
  ]
}
```



