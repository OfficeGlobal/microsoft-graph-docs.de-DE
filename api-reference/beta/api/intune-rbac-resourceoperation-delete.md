---
title: resourceOperation löschen
description: Löscht Objekte des Typs resourceOperation.
ms.openlocfilehash: 0bf2d4002856d16810f999f69ab6bf70e7e54d83
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27057948"
---
# <a name="delete-resourceoperation"></a><span data-ttu-id="b77c4-103">resourceOperation löschen</span><span class="sxs-lookup"><span data-stu-id="b77c4-103">Delete resourceOperation</span></span>

> <span data-ttu-id="b77c4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b77c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b77c4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b77c4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b77c4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b77c4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b77c4-107">Löscht Objekte des Typs [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b77c4-107">Deletes a [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b77c4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b77c4-108">Prerequisites</span></span>
<span data-ttu-id="b77c4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b77c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b77c4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b77c4-111">Permission type</span></span>|<span data-ttu-id="b77c4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b77c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b77c4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b77c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b77c4-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b77c4-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b77c4-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b77c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b77c4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b77c4-116">Not supported.</span></span>|
|<span data-ttu-id="b77c4-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b77c4-117">Application</span></span>|<span data-ttu-id="b77c4-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b77c4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b77c4-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b77c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="b77c4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b77c4-120">Request headers</span></span>
|<span data-ttu-id="b77c4-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b77c4-121">Header</span></span>|<span data-ttu-id="b77c4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b77c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b77c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b77c4-123">Authorization</span></span>|<span data-ttu-id="b77c4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b77c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b77c4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b77c4-125">Accept</span></span>|<span data-ttu-id="b77c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b77c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b77c4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b77c4-127">Request body</span></span>
<span data-ttu-id="b77c4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b77c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b77c4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="b77c4-129">Response</span></span>
<span data-ttu-id="b77c4-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b77c4-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b77c4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b77c4-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b77c4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b77c4-132">Request</span></span>
<span data-ttu-id="b77c4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b77c4-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
```

### <a name="response"></a><span data-ttu-id="b77c4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b77c4-134">Response</span></span>
<span data-ttu-id="b77c4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b77c4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





