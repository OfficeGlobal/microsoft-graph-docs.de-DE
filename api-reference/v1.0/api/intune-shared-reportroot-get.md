---
title: Abrufen von „reportRoot“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e24a86c1ff4443b0d2867dc9f7da7e273a3012e0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251909"
---
# <a name="get-reportroot"></a><span data-ttu-id="1abc2-103">Abrufen von „reportRoot“</span><span class="sxs-lookup"><span data-stu-id="1abc2-103">Get reportRoot</span></span>

> <span data-ttu-id="1abc2-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1abc2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1abc2-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="1abc2-105">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1abc2-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1abc2-106">Prerequisites</span></span>
<span data-ttu-id="1abc2-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1abc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1abc2-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1abc2-109">Permission type</span></span>|<span data-ttu-id="1abc2-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1abc2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1abc2-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1abc2-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1abc2-112">&nbsp;&nbsp; Gerätekonfiguration</span><span class="sxs-lookup"><span data-stu-id="1abc2-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="1abc2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1abc2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="1abc2-114">&nbsp;&nbsp; Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="1abc2-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="1abc2-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1abc2-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1abc2-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1abc2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1abc2-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1abc2-117">Not supported.</span></span>|
|<span data-ttu-id="1abc2-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1abc2-118">Application</span></span>|<span data-ttu-id="1abc2-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1abc2-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1abc2-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1abc2-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1abc2-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1abc2-121">Optional query parameters</span></span>
<span data-ttu-id="1abc2-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1abc2-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1abc2-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1abc2-123">Request headers</span></span>
|<span data-ttu-id="1abc2-124">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1abc2-124">Header</span></span>|<span data-ttu-id="1abc2-125">Wert</span><span class="sxs-lookup"><span data-stu-id="1abc2-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1abc2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1abc2-126">Authorization</span></span>|<span data-ttu-id="1abc2-127">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1abc2-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1abc2-128">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1abc2-128">Accept</span></span>|<span data-ttu-id="1abc2-129">application/json</span><span class="sxs-lookup"><span data-stu-id="1abc2-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1abc2-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1abc2-130">Request body</span></span>
<span data-ttu-id="1abc2-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1abc2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1abc2-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1abc2-132">Response</span></span>
<span data-ttu-id="1abc2-133">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [reportRoot](../resources/intune-shared-reportroot.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1abc2-133">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1abc2-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1abc2-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="1abc2-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1abc2-135">Request</span></span>
<span data-ttu-id="1abc2-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1abc2-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="1abc2-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="1abc2-137">Response</span></span>
<span data-ttu-id="1abc2-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1abc2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```








