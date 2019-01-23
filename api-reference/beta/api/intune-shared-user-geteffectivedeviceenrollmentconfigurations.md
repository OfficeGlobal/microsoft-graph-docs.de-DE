---
title: GetEffectiveDeviceEnrollmentConfigurations-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ee8eb2ff3a15d234d05ed28a13f600e7e47e4d53
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399780"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="80f39-103">GetEffectiveDeviceEnrollmentConfigurations-Funktion</span><span class="sxs-lookup"><span data-stu-id="80f39-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="80f39-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="80f39-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="80f39-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80f39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80f39-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="80f39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80f39-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="80f39-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80f39-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="80f39-108">Prerequisites</span></span>

<span data-ttu-id="80f39-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80f39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80f39-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="80f39-111">Permission type</span></span>|<span data-ttu-id="80f39-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="80f39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80f39-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="80f39-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="80f39-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="80f39-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="80f39-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80f39-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="80f39-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="80f39-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80f39-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80f39-117">Not supported.</span></span>|
|<span data-ttu-id="80f39-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="80f39-118">Application</span></span>|<span data-ttu-id="80f39-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="80f39-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80f39-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="80f39-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="80f39-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="80f39-121">Request headers</span></span>

|<span data-ttu-id="80f39-122">Header</span><span class="sxs-lookup"><span data-stu-id="80f39-122">Header</span></span>|<span data-ttu-id="80f39-123">Wert</span><span class="sxs-lookup"><span data-stu-id="80f39-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80f39-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="80f39-124">Authorization</span></span>|<span data-ttu-id="80f39-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="80f39-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80f39-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="80f39-126">Accept</span></span>|<span data-ttu-id="80f39-127">application/json</span><span class="sxs-lookup"><span data-stu-id="80f39-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80f39-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="80f39-128">Request body</span></span>

<span data-ttu-id="80f39-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="80f39-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80f39-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="80f39-130">Response</span></span>

<span data-ttu-id="80f39-131">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="80f39-131">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80f39-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="80f39-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="80f39-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="80f39-133">Request</span></span>

<span data-ttu-id="80f39-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="80f39-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="80f39-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="80f39-135">Response</span></span>

<span data-ttu-id="80f39-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="80f39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```



