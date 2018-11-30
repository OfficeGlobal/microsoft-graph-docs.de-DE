---
title: Auflisten von „deviceEnrollmentWindowsHelloForBusinessConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceEnrollmentWindowsHelloForBusinessConfiguration auf.
ms.openlocfilehash: be1e717a03daecc1f9c37ad00831cd1413781f2e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017453"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="ce04c-103">Auflisten von „deviceEnrollmentWindowsHelloForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="ce04c-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

> <span data-ttu-id="ce04c-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ce04c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce04c-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="ce04c-105">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce04c-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ce04c-106">Prerequisites</span></span>
<span data-ttu-id="ce04c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce04c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce04c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ce04c-109">Permission type</span></span>|<span data-ttu-id="ce04c-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ce04c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce04c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ce04c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce04c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce04c-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ce04c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ce04c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce04c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce04c-114">Not supported.</span></span>|
|<span data-ttu-id="ce04c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ce04c-115">Application</span></span>|<span data-ttu-id="ce04c-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ce04c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce04c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce04c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ce04c-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ce04c-118">Request headers</span></span>
|<span data-ttu-id="ce04c-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ce04c-119">Header</span></span>|<span data-ttu-id="ce04c-120">Wert</span><span class="sxs-lookup"><span data-stu-id="ce04c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce04c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce04c-121">Authorization</span></span>|<span data-ttu-id="ce04c-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ce04c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce04c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ce04c-123">Accept</span></span>|<span data-ttu-id="ce04c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ce04c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce04c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ce04c-125">Request body</span></span>
<span data-ttu-id="ce04c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ce04c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce04c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce04c-127">Response</span></span>
<span data-ttu-id="ce04c-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ce04c-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce04c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ce04c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce04c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ce04c-130">Request</span></span>
<span data-ttu-id="ce04c-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ce04c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="ce04c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="ce04c-132">Response</span></span>
<span data-ttu-id="ce04c-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ce04c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
      "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "pinMinimumLength": 0,
      "pinMaximumLength": 0,
      "pinUppercaseCharactersUsage": "required",
      "pinLowercaseCharactersUsage": "required",
      "pinSpecialCharactersUsage": "required",
      "state": "enabled",
      "securityDeviceRequired": true,
      "unlockWithBiometricsEnabled": true,
      "remotePassportEnabled": true,
      "pinPreviousBlockCount": 5,
      "pinExpirationInDays": 3,
      "enhancedBiometricsState": "enabled"
    }
  ]
}
```



