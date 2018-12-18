---
title: Abrufen von „managedEBookAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedEBookAssignment.
author: tfitzmac
ms.openlocfilehash: ea88a296849d109ac6a38fa39774d5be7be18133
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323023"
---
# <a name="get-managedebookassignment"></a><span data-ttu-id="09e66-103">Abrufen von „managedEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="09e66-103">Get managedEBookAssignment</span></span>

> <span data-ttu-id="09e66-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="09e66-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09e66-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="09e66-105">Read properties and relationships of the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="09e66-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="09e66-106">Prerequisites</span></span>
<span data-ttu-id="09e66-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09e66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09e66-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="09e66-109">Permission type</span></span>|<span data-ttu-id="09e66-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="09e66-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09e66-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="09e66-111">Delegated (work or school account)</span></span>|<span data-ttu-id="09e66-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="09e66-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="09e66-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="09e66-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09e66-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09e66-114">Not supported.</span></span>|
|<span data-ttu-id="09e66-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="09e66-115">Application</span></span>|<span data-ttu-id="09e66-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="09e66-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09e66-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="09e66-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09e66-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="09e66-118">Optional query parameters</span></span>
<span data-ttu-id="09e66-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="09e66-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="09e66-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="09e66-120">Request headers</span></span>
|<span data-ttu-id="09e66-121">Header</span><span class="sxs-lookup"><span data-stu-id="09e66-121">Header</span></span>|<span data-ttu-id="09e66-122">Wert</span><span class="sxs-lookup"><span data-stu-id="09e66-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09e66-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="09e66-123">Authorization</span></span>|<span data-ttu-id="09e66-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="09e66-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09e66-125">Accept</span><span class="sxs-lookup"><span data-stu-id="09e66-125">Accept</span></span>|<span data-ttu-id="09e66-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09e66-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09e66-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="09e66-127">Request body</span></span>
<span data-ttu-id="09e66-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="09e66-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09e66-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="09e66-129">Response</span></span>
<span data-ttu-id="09e66-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="09e66-130">If successful, this method returns a `200 OK` response code and [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09e66-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="09e66-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="09e66-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09e66-132">Request</span></span>
<span data-ttu-id="09e66-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="09e66-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="09e66-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="09e66-134">Response</span></span>
<span data-ttu-id="09e66-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="09e66-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBookAssignment",
    "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "installIntent": "required"
  }
}
```



