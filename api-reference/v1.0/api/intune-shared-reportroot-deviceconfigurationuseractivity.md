---
title: Funktion „deviceConfigurationUserActivity“
description: Metadaten für den Benutzeraktivitätsbericht zu einer Gerätekonfiguration
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2ecafdc399eab5150b80d83a68bdb6086dfa486
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849077"
---
# <a name="deviceconfigurationuseractivity-function"></a><span data-ttu-id="2e522-103">Funktion „deviceConfigurationUserActivity“</span><span class="sxs-lookup"><span data-stu-id="2e522-103">deviceConfigurationUserActivity function</span></span>

> <span data-ttu-id="2e522-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2e522-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e522-105">Metadaten für den Benutzeraktivitätsbericht zu einer Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="2e522-105">Metadata for the device configuration user activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e522-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2e522-106">Prerequisites</span></span>
<span data-ttu-id="2e522-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e522-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e522-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e522-109">Permission type</span></span>|<span data-ttu-id="2e522-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e522-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e522-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e522-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2e522-112">&nbsp;&nbsp; Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="2e522-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="2e522-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e522-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2e522-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e522-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e522-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e522-115">Not supported.</span></span>|
|<span data-ttu-id="2e522-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e522-116">Application</span></span>|<span data-ttu-id="2e522-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e522-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e522-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e522-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationUserActivity
```

## <a name="request-headers"></a><span data-ttu-id="2e522-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e522-119">Request headers</span></span>
|<span data-ttu-id="2e522-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2e522-120">Header</span></span>|<span data-ttu-id="2e522-121">Wert</span><span class="sxs-lookup"><span data-stu-id="2e522-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e522-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e522-122">Authorization</span></span>|<span data-ttu-id="2e522-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2e522-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e522-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2e522-124">Accept</span></span>|<span data-ttu-id="2e522-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2e522-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e522-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e522-126">Request body</span></span>
<span data-ttu-id="2e522-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2e522-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e522-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e522-128">Response</span></span>
<span data-ttu-id="2e522-129">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und einen [Bericht](../resources/intune-shared-report.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="2e522-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e522-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e522-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e522-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e522-131">Request</span></span>
<span data-ttu-id="2e522-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e522-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationUserActivity
```

### <a name="response"></a><span data-ttu-id="2e522-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e522-133">Response</span></span>
<span data-ttu-id="2e522-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e522-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








