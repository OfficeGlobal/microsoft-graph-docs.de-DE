---
title: deviceConfigurationDeviceActivity-Funktion
description: Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b0b9231b119365290259cd1eb97f0659766d0586
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170805"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="7c1c8-103">deviceConfigurationDeviceActivity-Funktion</span><span class="sxs-lookup"><span data-stu-id="7c1c8-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="7c1c8-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="7c1c8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7c1c8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7c1c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c1c8-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7c1c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c1c8-107">Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht</span><span class="sxs-lookup"><span data-stu-id="7c1c8-107">Metadata for the device configuration device activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7c1c8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7c1c8-108">Prerequisites</span></span>
<span data-ttu-id="7c1c8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c1c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="7c1c8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7c1c8-111">Permission type</span></span>|<span data-ttu-id="7c1c8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7c1c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c1c8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7c1c8-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7c1c8-114">&nbsp; &nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="7c1c8-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="7c1c8-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c1c8-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7c1c8-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7c1c8-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c1c8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c1c8-117">Not supported.</span></span>|
|<span data-ttu-id="7c1c8-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7c1c8-118">Application</span></span>|<span data-ttu-id="7c1c8-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7c1c8-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c1c8-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c1c8-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="7c1c8-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7c1c8-121">Request headers</span></span>
|<span data-ttu-id="7c1c8-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7c1c8-122">Header</span></span>|<span data-ttu-id="7c1c8-123">Wert</span><span class="sxs-lookup"><span data-stu-id="7c1c8-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c1c8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c1c8-124">Authorization</span></span>|<span data-ttu-id="7c1c8-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7c1c8-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c1c8-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7c1c8-126">Accept</span></span>|<span data-ttu-id="7c1c8-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7c1c8-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c1c8-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7c1c8-128">Request body</span></span>
<span data-ttu-id="7c1c8-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7c1c8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c1c8-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c1c8-130">Response</span></span>
<span data-ttu-id="7c1c8-131">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7c1c8-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c1c8-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7c1c8-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="7c1c8-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7c1c8-133">Request</span></span>
<span data-ttu-id="7c1c8-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7c1c8-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="7c1c8-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="7c1c8-135">Response</span></span>
<span data-ttu-id="7c1c8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7c1c8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```



