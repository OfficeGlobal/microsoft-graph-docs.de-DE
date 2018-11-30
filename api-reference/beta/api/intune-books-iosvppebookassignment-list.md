---
title: Auflisten von „iosVppEBookAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs iosVppEBookAssignment auf.
ms.openlocfilehash: 3de4f0510a692dcff41212b8f96db6d99a0f5a11
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065394"
---
# <a name="list-iosvppebookassignments"></a><span data-ttu-id="eb3a0-103">Auflisten von „iosVppEBookAssignment“</span><span class="sxs-lookup"><span data-stu-id="eb3a0-103">List iosVppEBookAssignments</span></span>

> <span data-ttu-id="eb3a0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eb3a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb3a0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eb3a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb3a0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="eb3a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb3a0-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="eb3a0-107">List properties and relationships of the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb3a0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eb3a0-108">Prerequisites</span></span>
<span data-ttu-id="eb3a0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb3a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb3a0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb3a0-111">Permission type</span></span>|<span data-ttu-id="eb3a0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb3a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb3a0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb3a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eb3a0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb3a0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="eb3a0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb3a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb3a0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb3a0-116">Not supported.</span></span>|
|<span data-ttu-id="eb3a0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb3a0-117">Application</span></span>|<span data-ttu-id="eb3a0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb3a0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb3a0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb3a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="eb3a0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb3a0-120">Request headers</span></span>
|<span data-ttu-id="eb3a0-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eb3a0-121">Header</span></span>|<span data-ttu-id="eb3a0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="eb3a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb3a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb3a0-123">Authorization</span></span>|<span data-ttu-id="eb3a0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eb3a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb3a0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eb3a0-125">Accept</span></span>|<span data-ttu-id="eb3a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eb3a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb3a0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb3a0-127">Request body</span></span>
<span data-ttu-id="eb3a0-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eb3a0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb3a0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb3a0-129">Response</span></span>
<span data-ttu-id="eb3a0-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="eb3a0-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb3a0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb3a0-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb3a0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb3a0-132">Request</span></span>
<span data-ttu-id="eb3a0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb3a0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

### <a name="response"></a><span data-ttu-id="eb3a0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb3a0-134">Response</span></span>
<span data-ttu-id="eb3a0-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb3a0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





