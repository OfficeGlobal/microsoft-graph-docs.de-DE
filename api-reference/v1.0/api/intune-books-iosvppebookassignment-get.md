---
title: Abrufen von „iosVppEBookAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs iosVppEBookAssignment.
author: tfitzmac
ms.openlocfilehash: 73fd0914b7aa1c77907ee469cc1a9aeef54a7eed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305929"
---
# <a name="get-iosvppebookassignment"></a><span data-ttu-id="debfb-103">Abrufen von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="debfb-103">Get iosVppEBookAssignment</span></span>

> <span data-ttu-id="debfb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="debfb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="debfb-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="debfb-105">Read properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="debfb-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="debfb-106">Prerequisites</span></span>
<span data-ttu-id="debfb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="debfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="debfb-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="debfb-109">Permission type</span></span>|<span data-ttu-id="debfb-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="debfb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="debfb-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="debfb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="debfb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="debfb-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="debfb-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="debfb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="debfb-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="debfb-114">Not supported.</span></span>|
|<span data-ttu-id="debfb-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="debfb-115">Application</span></span>|<span data-ttu-id="debfb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="debfb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="debfb-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="debfb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="debfb-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="debfb-118">Optional query parameters</span></span>
<span data-ttu-id="debfb-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="debfb-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="debfb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="debfb-120">Request headers</span></span>
|<span data-ttu-id="debfb-121">Header</span><span class="sxs-lookup"><span data-stu-id="debfb-121">Header</span></span>|<span data-ttu-id="debfb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="debfb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="debfb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="debfb-123">Authorization</span></span>|<span data-ttu-id="debfb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="debfb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="debfb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="debfb-125">Accept</span></span>|<span data-ttu-id="debfb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="debfb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="debfb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="debfb-127">Request body</span></span>
<span data-ttu-id="debfb-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="debfb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="debfb-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="debfb-129">Response</span></span>
<span data-ttu-id="debfb-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="debfb-130">If successful, this method returns a `200 OK` response code and [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="debfb-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="debfb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="debfb-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="debfb-132">Request</span></span>
<span data-ttu-id="debfb-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="debfb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="debfb-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="debfb-134">Response</span></span>
<span data-ttu-id="debfb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="debfb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
    "id": "48f05789-5789-48f0-8957-f0488957f048",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "installIntent": "required"
  }
}
```



