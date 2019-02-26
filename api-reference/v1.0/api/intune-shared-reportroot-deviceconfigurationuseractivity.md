---
title: Funktion „deviceConfigurationUserActivity“
description: Metadaten für den Benutzeraktivitätsbericht zu einer Gerätekonfiguration
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c83c9a6216e678d16af212f6a31648f7dea8a2b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258023"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="45979-103">Funktion „deviceConfigurationUserActivity“</span><span class="sxs-lookup"><span data-stu-id="45979-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="45979-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="45979-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45979-105">Metadaten für den Benutzeraktivitätsbericht zu einer Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="45979-105">Metadata for the device configuration user activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45979-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="45979-106">Prerequisites</span></span>
<span data-ttu-id="45979-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45979-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45979-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="45979-109">Permission type</span></span>|<span data-ttu-id="45979-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="45979-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45979-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="45979-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="45979-112">&nbsp;&nbsp; Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="45979-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="45979-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="45979-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="45979-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="45979-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45979-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45979-115">Not supported.</span></span>|
|<span data-ttu-id="45979-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="45979-116">Application</span></span>|<span data-ttu-id="45979-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45979-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45979-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="45979-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="45979-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="45979-119">Request headers</span></span>
|<span data-ttu-id="45979-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="45979-120">Header</span></span>|<span data-ttu-id="45979-121">Wert</span><span class="sxs-lookup"><span data-stu-id="45979-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45979-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45979-122">Authorization</span></span>|<span data-ttu-id="45979-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="45979-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45979-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="45979-124">Accept</span></span>|<span data-ttu-id="45979-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45979-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45979-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="45979-126">Request body</span></span>
<span data-ttu-id="45979-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="45979-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45979-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="45979-128">Response</span></span>
<span data-ttu-id="45979-129">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="45979-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45979-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="45979-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="45979-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="45979-131">Request</span></span>
<span data-ttu-id="45979-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="45979-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="45979-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="45979-133">Response</span></span>
<span data-ttu-id="45979-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="45979-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








