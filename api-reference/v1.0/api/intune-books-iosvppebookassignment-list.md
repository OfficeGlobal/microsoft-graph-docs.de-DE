---
title: Auflisten von „iosVppEBookAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosVppEBookAssignment auf.
ms.openlocfilehash: f6e03361a3413c772517ab92deed6e7c9dc2322b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016299"
---
# <a name="list-iosvppebookassignments"></a><span data-ttu-id="1c9a8-103">Auflisten von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="1c9a8-103">List iosVppEBookAssignments</span></span>

> <span data-ttu-id="1c9a8-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="1c9a8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1c9a8-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="1c9a8-105">List properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1c9a8-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1c9a8-106">Prerequisites</span></span>
<span data-ttu-id="1c9a8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c9a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c9a8-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1c9a8-109">Permission type</span></span>|<span data-ttu-id="1c9a8-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1c9a8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c9a8-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1c9a8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1c9a8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c9a8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1c9a8-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1c9a8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c9a8-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c9a8-114">Not supported.</span></span>|
|<span data-ttu-id="1c9a8-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1c9a8-115">Application</span></span>|<span data-ttu-id="1c9a8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1c9a8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c9a8-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c9a8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1c9a8-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1c9a8-118">Request headers</span></span>
|<span data-ttu-id="1c9a8-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1c9a8-119">Header</span></span>|<span data-ttu-id="1c9a8-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1c9a8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c9a8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c9a8-121">Authorization</span></span>|<span data-ttu-id="1c9a8-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1c9a8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c9a8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1c9a8-123">Accept</span></span>|<span data-ttu-id="1c9a8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1c9a8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c9a8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1c9a8-125">Request body</span></span>
<span data-ttu-id="1c9a8-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1c9a8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c9a8-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c9a8-127">Response</span></span>
<span data-ttu-id="1c9a8-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1c9a8-128">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c9a8-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1c9a8-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1c9a8-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1c9a8-130">Request</span></span>
<span data-ttu-id="1c9a8-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1c9a8-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="1c9a8-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="1c9a8-132">Response</span></span>
<span data-ttu-id="1c9a8-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1c9a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 299

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
      "id": "48f05789-5789-48f0-8957-f0488957f048",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "installIntent": "required"
    }
  ]
}
```



