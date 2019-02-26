---
title: deviceConfigurationDeviceActivity-Funktion
description: Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a92ca929c45e9da34e598df079197fd76a2761bd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262097"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="57c3e-103">deviceConfigurationDeviceActivity-Funktion</span><span class="sxs-lookup"><span data-stu-id="57c3e-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="57c3e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="57c3e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57c3e-105">Metadaten für den Gerätekonfigurations-Geräteaktivitätsbericht</span><span class="sxs-lookup"><span data-stu-id="57c3e-105">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57c3e-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="57c3e-106">Prerequisites</span></span>
<span data-ttu-id="57c3e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57c3e-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="57c3e-109">Permission type</span></span>|<span data-ttu-id="57c3e-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="57c3e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57c3e-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="57c3e-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="57c3e-112">&nbsp;&nbsp; Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="57c3e-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="57c3e-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="57c3e-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="57c3e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="57c3e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57c3e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57c3e-115">Not supported.</span></span>|
|<span data-ttu-id="57c3e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="57c3e-116">Application</span></span>|<span data-ttu-id="57c3e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57c3e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57c3e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="57c3e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="57c3e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="57c3e-119">Request headers</span></span>
|<span data-ttu-id="57c3e-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="57c3e-120">Header</span></span>|<span data-ttu-id="57c3e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="57c3e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57c3e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="57c3e-122">Authorization</span></span>|<span data-ttu-id="57c3e-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="57c3e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57c3e-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="57c3e-124">Accept</span></span>|<span data-ttu-id="57c3e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57c3e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57c3e-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="57c3e-126">Request body</span></span>
<span data-ttu-id="57c3e-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="57c3e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57c3e-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="57c3e-128">Response</span></span>
<span data-ttu-id="57c3e-129">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="57c3e-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57c3e-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="57c3e-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="57c3e-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="57c3e-131">Request</span></span>
<span data-ttu-id="57c3e-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="57c3e-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="57c3e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="57c3e-133">Response</span></span>
<span data-ttu-id="57c3e-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="57c3e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








