---
title: Abrufen von „managedAppStatus“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppStatus.
ms.openlocfilehash: ee2beeda26b27c2497e9aadcf35731568fc5869d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017339"
---
# <a name="get-managedappstatus"></a><span data-ttu-id="55409-103">Abrufen von „managedAppStatus“</span><span class="sxs-lookup"><span data-stu-id="55409-103">Get managedAppStatus</span></span>

> <span data-ttu-id="55409-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="55409-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55409-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="55409-105">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="55409-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="55409-106">Prerequisites</span></span>
<span data-ttu-id="55409-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55409-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55409-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="55409-109">Permission type</span></span>|<span data-ttu-id="55409-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="55409-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55409-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="55409-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55409-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="55409-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="55409-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="55409-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55409-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55409-114">Not supported.</span></span>|
|<span data-ttu-id="55409-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="55409-115">Application</span></span>|<span data-ttu-id="55409-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55409-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55409-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="55409-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55409-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="55409-118">Optional query parameters</span></span>
<span data-ttu-id="55409-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="55409-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="55409-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="55409-120">Request headers</span></span>
|<span data-ttu-id="55409-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="55409-121">Header</span></span>|<span data-ttu-id="55409-122">Wert</span><span class="sxs-lookup"><span data-stu-id="55409-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55409-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55409-123">Authorization</span></span>|<span data-ttu-id="55409-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="55409-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55409-125">Accept</span><span class="sxs-lookup"><span data-stu-id="55409-125">Accept</span></span>|<span data-ttu-id="55409-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55409-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55409-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="55409-127">Request body</span></span>
<span data-ttu-id="55409-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="55409-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55409-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="55409-129">Response</span></span>
<span data-ttu-id="55409-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppStatus](../resources/intune-mam-managedappstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="55409-130">If successful, this method returns a `200 OK` response code and [managedAppStatus](../resources/intune-mam-managedappstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55409-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="55409-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="55409-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="55409-132">Request</span></span>
<span data-ttu-id="55409-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="55409-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="55409-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="55409-134">Response</span></span>
<span data-ttu-id="55409-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="55409-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppStatus",
    "displayName": "Display Name value",
    "id": "ad1f7541-7541-ad1f-4175-1fad41751fad",
    "version": "Version value"
  }
}
```



