---
title: Auflisten von „deviceEnrollmentWindowsHelloForBusinessConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceEnrollmentWindowsHelloForBusinessConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f40a646e18e5cecb40361952c14021331902644
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861397"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="fa67e-103">Auflisten von „deviceEnrollmentWindowsHelloForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="fa67e-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

> <span data-ttu-id="fa67e-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fa67e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa67e-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="fa67e-105">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa67e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa67e-106">Prerequisites</span></span>
<span data-ttu-id="fa67e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa67e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa67e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa67e-109">Permission type</span></span>|<span data-ttu-id="fa67e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa67e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa67e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa67e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa67e-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa67e-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fa67e-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa67e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa67e-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa67e-114">Not supported.</span></span>|
|<span data-ttu-id="fa67e-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa67e-115">Application</span></span>|<span data-ttu-id="fa67e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa67e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa67e-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa67e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa67e-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa67e-118">Request headers</span></span>
|<span data-ttu-id="fa67e-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fa67e-119">Header</span></span>|<span data-ttu-id="fa67e-120">Wert</span><span class="sxs-lookup"><span data-stu-id="fa67e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa67e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa67e-121">Authorization</span></span>|<span data-ttu-id="fa67e-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa67e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa67e-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fa67e-123">Accept</span></span>|<span data-ttu-id="fa67e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fa67e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa67e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa67e-125">Request body</span></span>
<span data-ttu-id="fa67e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fa67e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa67e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa67e-127">Response</span></span>
<span data-ttu-id="fa67e-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fa67e-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa67e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa67e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa67e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa67e-130">Request</span></span>
<span data-ttu-id="fa67e-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa67e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="fa67e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa67e-132">Response</span></span>
<span data-ttu-id="fa67e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa67e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



