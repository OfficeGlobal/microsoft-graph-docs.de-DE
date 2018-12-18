---
title: Abrufen von „deviceEnrollmentWindowsHelloForBusinessConfiguration“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: tfitzmac
ms.openlocfilehash: a5ee2052854582c6892f6609647207fbe9d9c358
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361201"
---
# <a name="get-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="5cc67-103">Abrufen von „deviceEnrollmentWindowsHelloForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="5cc67-103">Get deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="5cc67-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5cc67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cc67-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5cc67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cc67-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5cc67-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cc67-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5cc67-107">Read properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5cc67-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5cc67-108">Prerequisites</span></span>
<span data-ttu-id="5cc67-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cc67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cc67-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5cc67-111">Permission type</span></span>|<span data-ttu-id="5cc67-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5cc67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cc67-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5cc67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cc67-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cc67-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="5cc67-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5cc67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cc67-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5cc67-116">Not supported.</span></span>|
|<span data-ttu-id="5cc67-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5cc67-117">Application</span></span>|<span data-ttu-id="5cc67-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5cc67-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cc67-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5cc67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5cc67-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5cc67-120">Optional query parameters</span></span>
<span data-ttu-id="5cc67-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5cc67-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5cc67-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5cc67-122">Request headers</span></span>
|<span data-ttu-id="5cc67-123">Header</span><span class="sxs-lookup"><span data-stu-id="5cc67-123">Header</span></span>|<span data-ttu-id="5cc67-124">Wert</span><span class="sxs-lookup"><span data-stu-id="5cc67-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cc67-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5cc67-125">Authorization</span></span>|<span data-ttu-id="5cc67-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5cc67-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cc67-127">Accept</span><span class="sxs-lookup"><span data-stu-id="5cc67-127">Accept</span></span>|<span data-ttu-id="5cc67-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5cc67-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cc67-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5cc67-129">Request body</span></span>
<span data-ttu-id="5cc67-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5cc67-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cc67-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5cc67-131">Response</span></span>
<span data-ttu-id="5cc67-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="5cc67-132">If successful, this method returns a `200 OK` response code and [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cc67-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5cc67-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="5cc67-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5cc67-134">Request</span></span>
<span data-ttu-id="5cc67-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5cc67-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5cc67-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5cc67-136">Response</span></span>
<span data-ttu-id="5cc67-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5cc67-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





