---
title: Abrufen von „managedAppStatusRaw“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppStatusRaw.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9de49cf70de0e75036d10a17f99d8bc68934a563
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920485"
---
# <a name="get-managedappstatusraw"></a><span data-ttu-id="cf4bb-103">Abrufen von „managedAppStatusRaw“</span><span class="sxs-lookup"><span data-stu-id="cf4bb-103">Get managedAppStatusRaw</span></span>

> <span data-ttu-id="cf4bb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cf4bb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf4bb-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="cf4bb-105">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf4bb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cf4bb-106">Prerequisites</span></span>
<span data-ttu-id="cf4bb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf4bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf4bb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf4bb-109">Permission type</span></span>|<span data-ttu-id="cf4bb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf4bb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf4bb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf4bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf4bb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf4bb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cf4bb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf4bb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf4bb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf4bb-114">Not supported.</span></span>|
|<span data-ttu-id="cf4bb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf4bb-115">Application</span></span>|<span data-ttu-id="cf4bb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf4bb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf4bb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf4bb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf4bb-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cf4bb-118">Optional query parameters</span></span>
<span data-ttu-id="cf4bb-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cf4bb-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cf4bb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf4bb-120">Request headers</span></span>
|<span data-ttu-id="cf4bb-121">Header</span><span class="sxs-lookup"><span data-stu-id="cf4bb-121">Header</span></span>|<span data-ttu-id="cf4bb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="cf4bb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf4bb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf4bb-123">Authorization</span></span>|<span data-ttu-id="cf4bb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cf4bb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf4bb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cf4bb-125">Accept</span></span>|<span data-ttu-id="cf4bb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf4bb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf4bb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf4bb-127">Request body</span></span>
<span data-ttu-id="cf4bb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cf4bb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf4bb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf4bb-129">Response</span></span>
<span data-ttu-id="cf4bb-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cf4bb-130">If successful, this method returns a `200 OK` response code and [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf4bb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf4bb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf4bb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf4bb-132">Request</span></span>
<span data-ttu-id="cf4bb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf4bb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="cf4bb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf4bb-134">Response</span></span>
<span data-ttu-id="cf4bb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf4bb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



