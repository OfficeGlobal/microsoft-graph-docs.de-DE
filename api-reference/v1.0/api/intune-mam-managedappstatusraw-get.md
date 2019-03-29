---
title: Abrufen von „managedAppStatusRaw“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppStatusRaw.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 897d5398a87a2cb451f9c0cc5408aeb7c953478a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966880"
---
# <a name="get-managedappstatusraw"></a><span data-ttu-id="fb136-103">Abrufen von „managedAppStatusRaw“</span><span class="sxs-lookup"><span data-stu-id="fb136-103">Get managedAppStatusRaw</span></span>

> <span data-ttu-id="fb136-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fb136-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb136-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="fb136-105">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb136-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fb136-106">Prerequisites</span></span>
<span data-ttu-id="fb136-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb136-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb136-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fb136-109">Permission type</span></span>|<span data-ttu-id="fb136-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fb136-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb136-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fb136-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fb136-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fb136-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fb136-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fb136-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb136-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fb136-114">Not supported.</span></span>|
|<span data-ttu-id="fb136-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fb136-115">Application</span></span>|<span data-ttu-id="fb136-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fb136-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb136-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fb136-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fb136-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fb136-118">Optional query parameters</span></span>
<span data-ttu-id="fb136-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fb136-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fb136-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fb136-120">Request headers</span></span>
|<span data-ttu-id="fb136-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fb136-121">Header</span></span>|<span data-ttu-id="fb136-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fb136-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb136-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb136-123">Authorization</span></span>|<span data-ttu-id="fb136-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fb136-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb136-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fb136-125">Accept</span></span>|<span data-ttu-id="fb136-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb136-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb136-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fb136-127">Request body</span></span>
<span data-ttu-id="fb136-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fb136-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb136-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="fb136-129">Response</span></span>
<span data-ttu-id="fb136-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fb136-130">If successful, this method returns a `200 OK` response code and [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb136-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fb136-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb136-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fb136-132">Request</span></span>
<span data-ttu-id="fb136-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fb136-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="fb136-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="fb136-134">Response</span></span>
<span data-ttu-id="fb136-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fb136-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppStatusRaw",
    "displayName": "Display Name value",
    "id": "80847581-7581-8084-8175-848081758480",
    "version": "Version value",
    "content": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```



