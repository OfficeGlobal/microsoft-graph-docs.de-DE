---
title: Abrufen von „iosVppEBookAssignment“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs iosVppEBookAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d1fbdbe44415dba3395e4a10b10d7a6e946a6ea3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823114"
---
# <a name="get-iosvppebookassignment"></a><span data-ttu-id="b5fe1-103">Abrufen von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="b5fe1-103">Get iosVppEBookAssignment</span></span>

> <span data-ttu-id="b5fe1-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b5fe1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5fe1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b5fe1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5fe1-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b5fe1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5fe1-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b5fe1-107">Read properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5fe1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b5fe1-108">Prerequisites</span></span>
<span data-ttu-id="b5fe1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5fe1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5fe1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b5fe1-111">Permission type</span></span>|<span data-ttu-id="b5fe1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b5fe1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5fe1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b5fe1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5fe1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5fe1-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b5fe1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b5fe1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5fe1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5fe1-116">Not supported.</span></span>|
|<span data-ttu-id="b5fe1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b5fe1-117">Application</span></span>|<span data-ttu-id="b5fe1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b5fe1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5fe1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5fe1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5fe1-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b5fe1-120">Optional query parameters</span></span>
<span data-ttu-id="b5fe1-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b5fe1-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b5fe1-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b5fe1-122">Request headers</span></span>
|<span data-ttu-id="b5fe1-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b5fe1-123">Header</span></span>|<span data-ttu-id="b5fe1-124">Wert</span><span class="sxs-lookup"><span data-stu-id="b5fe1-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5fe1-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5fe1-125">Authorization</span></span>|<span data-ttu-id="b5fe1-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b5fe1-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5fe1-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b5fe1-127">Accept</span></span>|<span data-ttu-id="b5fe1-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b5fe1-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5fe1-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b5fe1-129">Request body</span></span>
<span data-ttu-id="b5fe1-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b5fe1-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5fe1-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5fe1-131">Response</span></span>
<span data-ttu-id="b5fe1-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b5fe1-132">If successful, this method returns a `200 OK` response code and [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5fe1-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b5fe1-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5fe1-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b5fe1-134">Request</span></span>
<span data-ttu-id="b5fe1-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b5fe1-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="b5fe1-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b5fe1-136">Response</span></span>
<span data-ttu-id="b5fe1-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b5fe1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





