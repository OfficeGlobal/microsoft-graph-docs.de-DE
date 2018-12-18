---
title: GetEffectiveDeviceEnrollmentConfigurations-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: b7bdf815f972f56892027a01db83539065fe9caf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315253"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="20345-103">GetEffectiveDeviceEnrollmentConfigurations-Funktion</span><span class="sxs-lookup"><span data-stu-id="20345-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="20345-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="20345-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20345-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="20345-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20345-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="20345-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20345-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="20345-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20345-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="20345-108">Prerequisites</span></span>

<span data-ttu-id="20345-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20345-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20345-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="20345-111">Permission type</span></span>|<span data-ttu-id="20345-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="20345-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20345-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="20345-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="20345-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="20345-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="20345-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20345-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="20345-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="20345-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20345-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20345-117">Not supported.</span></span>|
|<span data-ttu-id="20345-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="20345-118">Application</span></span>|<span data-ttu-id="20345-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20345-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20345-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="20345-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="20345-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="20345-121">Request headers</span></span>

|<span data-ttu-id="20345-122">Header</span><span class="sxs-lookup"><span data-stu-id="20345-122">Header</span></span>|<span data-ttu-id="20345-123">Wert</span><span class="sxs-lookup"><span data-stu-id="20345-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20345-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="20345-124">Authorization</span></span>|<span data-ttu-id="20345-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="20345-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20345-126">Accept</span><span class="sxs-lookup"><span data-stu-id="20345-126">Accept</span></span>|<span data-ttu-id="20345-127">application/json</span><span class="sxs-lookup"><span data-stu-id="20345-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20345-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="20345-128">Request body</span></span>

<span data-ttu-id="20345-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="20345-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20345-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="20345-130">Response</span></span>

<span data-ttu-id="20345-131">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="20345-131">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20345-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="20345-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="20345-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="20345-133">Request</span></span>

<span data-ttu-id="20345-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="20345-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="20345-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="20345-135">Response</span></span>

<span data-ttu-id="20345-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="20345-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



