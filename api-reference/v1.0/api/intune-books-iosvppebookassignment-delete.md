---
title: iosVppEBookAssignment löschen
description: Löscht ein iosVppEBookAssignment-Objekt.
ms.openlocfilehash: 4f791150eb14deaec79be82166e2695d7bb8fbce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019264"
---
# <a name="delete-iosvppebookassignment"></a><span data-ttu-id="7d340-103">iosVppEBookAssignment löschen</span><span class="sxs-lookup"><span data-stu-id="7d340-103">Delete iosVppEBookAssignment</span></span>

> <span data-ttu-id="7d340-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7d340-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d340-105">Löscht ein [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md)-Objekt.</span><span class="sxs-lookup"><span data-stu-id="7d340-105">Deletes a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d340-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7d340-106">Prerequisites</span></span>
<span data-ttu-id="7d340-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d340-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d340-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7d340-109">Permission type</span></span>|<span data-ttu-id="7d340-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7d340-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d340-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7d340-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d340-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d340-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d340-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7d340-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d340-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d340-114">Not supported.</span></span>|
|<span data-ttu-id="7d340-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7d340-115">Application</span></span>|<span data-ttu-id="7d340-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d340-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d340-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d340-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7d340-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7d340-118">Request headers</span></span>
|<span data-ttu-id="7d340-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7d340-119">Header</span></span>|<span data-ttu-id="7d340-120">Wert</span><span class="sxs-lookup"><span data-stu-id="7d340-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d340-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d340-121">Authorization</span></span>|<span data-ttu-id="7d340-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7d340-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d340-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7d340-123">Accept</span></span>|<span data-ttu-id="7d340-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7d340-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d340-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7d340-125">Request body</span></span>
<span data-ttu-id="7d340-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7d340-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d340-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d340-127">Response</span></span>
<span data-ttu-id="7d340-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7d340-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7d340-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7d340-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d340-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d340-130">Request</span></span>
<span data-ttu-id="7d340-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7d340-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

### <a name="response"></a><span data-ttu-id="7d340-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d340-132">Response</span></span>
<span data-ttu-id="7d340-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7d340-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



