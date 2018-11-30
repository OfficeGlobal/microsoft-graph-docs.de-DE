---
title: Abrufen von „deviceEnrollmentWindowsHelloForBusinessConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceEnrollmentWindowsHelloForBusinessConfiguration.
ms.openlocfilehash: ab801bc5e9a80d2998ae1bd6738f3b51ec11df1b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018070"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="ab980-103">Abrufen von „deviceEnrollmentWindowsHelloForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="ab980-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="ab980-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ab980-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab980-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ab980-105">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab980-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ab980-106">Prerequisites</span></span>
<span data-ttu-id="ab980-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab980-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab980-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ab980-109">Permission type</span></span>|<span data-ttu-id="ab980-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ab980-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab980-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ab980-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ab980-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab980-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ab980-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ab980-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab980-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab980-114">Not supported.</span></span>|
|<span data-ttu-id="ab980-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ab980-115">Application</span></span>|<span data-ttu-id="ab980-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab980-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab980-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab980-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab980-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ab980-118">Optional query parameters</span></span>
<span data-ttu-id="ab980-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ab980-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ab980-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ab980-120">Request headers</span></span>
|<span data-ttu-id="ab980-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ab980-121">Header</span></span>|<span data-ttu-id="ab980-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ab980-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab980-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab980-123">Authorization</span></span>|<span data-ttu-id="ab980-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ab980-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab980-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab980-125">Accept</span></span>|<span data-ttu-id="ab980-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab980-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab980-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ab980-127">Request body</span></span>
<span data-ttu-id="ab980-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ab980-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab980-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab980-129">Response</span></span>
<span data-ttu-id="ab980-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ab980-130">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab980-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ab980-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab980-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab980-132">Request</span></span>
<span data-ttu-id="ab980-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ab980-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ab980-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab980-134">Response</span></span>
<span data-ttu-id="ab980-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ab980-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 860

{
  "value": {
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
}
```


