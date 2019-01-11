---
title: Auflisten von „deviceEnrollmentWindowsHelloForBusinessConfiguration“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceEnrollmentWindowsHelloForBusinessConfiguration auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2e7a620b007e1a28c18727bbcbc8e9fcd69dc8c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846690"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="dd0f3-103">Auflisten von „deviceEnrollmentWindowsHelloForBusinessConfiguration“</span><span class="sxs-lookup"><span data-stu-id="dd0f3-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

> <span data-ttu-id="dd0f3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="dd0f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd0f3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="dd0f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd0f3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="dd0f3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd0f3-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) auf.</span><span class="sxs-lookup"><span data-stu-id="dd0f3-107">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dd0f3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="dd0f3-108">Prerequisites</span></span>
<span data-ttu-id="dd0f3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd0f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd0f3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="dd0f3-111">Permission type</span></span>|<span data-ttu-id="dd0f3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="dd0f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd0f3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="dd0f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd0f3-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd0f3-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="dd0f3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="dd0f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd0f3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd0f3-116">Not supported.</span></span>|
|<span data-ttu-id="dd0f3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="dd0f3-117">Application</span></span>|<span data-ttu-id="dd0f3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="dd0f3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd0f3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd0f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dd0f3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="dd0f3-120">Request headers</span></span>
|<span data-ttu-id="dd0f3-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="dd0f3-121">Header</span></span>|<span data-ttu-id="dd0f3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="dd0f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd0f3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd0f3-123">Authorization</span></span>|<span data-ttu-id="dd0f3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="dd0f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd0f3-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="dd0f3-125">Accept</span></span>|<span data-ttu-id="dd0f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd0f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd0f3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="dd0f3-127">Request body</span></span>
<span data-ttu-id="dd0f3-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="dd0f3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd0f3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd0f3-129">Response</span></span>
<span data-ttu-id="dd0f3-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="dd0f3-130">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd0f3-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="dd0f3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="dd0f3-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="dd0f3-132">Request</span></span>
<span data-ttu-id="dd0f3-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="dd0f3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="dd0f3-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="dd0f3-134">Response</span></span>
<span data-ttu-id="dd0f3-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="dd0f3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





