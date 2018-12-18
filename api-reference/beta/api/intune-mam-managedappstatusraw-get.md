---
title: Abrufen von „managedAppStatusRaw“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppStatusRaw.
author: tfitzmac
ms.openlocfilehash: c308b36a49645b682b497f928c997eebdae6d520
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356182"
---
# <a name="get-managedappstatusraw"></a><span data-ttu-id="84bbb-103">Abrufen von „managedAppStatusRaw“</span><span class="sxs-lookup"><span data-stu-id="84bbb-103">Get managedAppStatusRaw</span></span>

> <span data-ttu-id="84bbb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="84bbb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84bbb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="84bbb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84bbb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="84bbb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84bbb-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="84bbb-107">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84bbb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="84bbb-108">Prerequisites</span></span>
<span data-ttu-id="84bbb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84bbb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84bbb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="84bbb-111">Permission type</span></span>|<span data-ttu-id="84bbb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="84bbb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84bbb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="84bbb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84bbb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="84bbb-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="84bbb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="84bbb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84bbb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84bbb-116">Not supported.</span></span>|
|<span data-ttu-id="84bbb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="84bbb-117">Application</span></span>|<span data-ttu-id="84bbb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="84bbb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84bbb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="84bbb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84bbb-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="84bbb-120">Optional query parameters</span></span>
<span data-ttu-id="84bbb-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="84bbb-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="84bbb-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="84bbb-122">Request headers</span></span>
|<span data-ttu-id="84bbb-123">Header</span><span class="sxs-lookup"><span data-stu-id="84bbb-123">Header</span></span>|<span data-ttu-id="84bbb-124">Wert</span><span class="sxs-lookup"><span data-stu-id="84bbb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84bbb-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="84bbb-125">Authorization</span></span>|<span data-ttu-id="84bbb-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="84bbb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84bbb-127">Accept</span><span class="sxs-lookup"><span data-stu-id="84bbb-127">Accept</span></span>|<span data-ttu-id="84bbb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="84bbb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84bbb-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="84bbb-129">Request body</span></span>
<span data-ttu-id="84bbb-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="84bbb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84bbb-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="84bbb-131">Response</span></span>
<span data-ttu-id="84bbb-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="84bbb-132">If successful, this method returns a `200 OK` response code and [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84bbb-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="84bbb-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="84bbb-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="84bbb-134">Request</span></span>
<span data-ttu-id="84bbb-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="84bbb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="84bbb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="84bbb-136">Response</span></span>
<span data-ttu-id="84bbb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="84bbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





