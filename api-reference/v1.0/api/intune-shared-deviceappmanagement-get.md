---
title: Abrufen von „deviceAppManagement“
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d700939f9073ff5d655421942ccc83ff5fc6bf7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935423"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="ab80b-103">Abrufen von „deviceAppManagement“</span><span class="sxs-lookup"><span data-stu-id="ab80b-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="ab80b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ab80b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab80b-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="ab80b-105">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab80b-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ab80b-106">Prerequisites</span></span>

<span data-ttu-id="ab80b-107">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="ab80b-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="ab80b-108">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab80b-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="ab80b-109">Beachten Sie, dass die entsprechende Berechtigungen gemäß den Workflow variiert.</span><span class="sxs-lookup"><span data-stu-id="ab80b-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="ab80b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ab80b-110">Permission type</span></span>|<span data-ttu-id="ab80b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ab80b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab80b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ab80b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ab80b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab80b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="ab80b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ab80b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab80b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab80b-115">Not supported.</span></span>|
|<span data-ttu-id="ab80b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ab80b-116">Application</span></span>|<span data-ttu-id="ab80b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ab80b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab80b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ab80b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab80b-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ab80b-119">Optional query parameters</span></span>
<span data-ttu-id="ab80b-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ab80b-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab80b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ab80b-121">Request headers</span></span>
|<span data-ttu-id="ab80b-122">Header</span><span class="sxs-lookup"><span data-stu-id="ab80b-122">Header</span></span>|<span data-ttu-id="ab80b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="ab80b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab80b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab80b-124">Authorization</span></span>|<span data-ttu-id="ab80b-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ab80b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab80b-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ab80b-126">Accept</span></span>|<span data-ttu-id="ab80b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ab80b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab80b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ab80b-128">Request body</span></span>
<span data-ttu-id="ab80b-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ab80b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab80b-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ab80b-130">Response</span></span>
<span data-ttu-id="ab80b-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ab80b-131">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="ab80b-132">Beispielanforderung</span><span class="sxs-lookup"><span data-stu-id="ab80b-132">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="ab80b-133">Beispielantwort</span><span class="sxs-lookup"><span data-stu-id="ab80b-133">Example response</span></span>
<span data-ttu-id="ab80b-134">Der Kürze halber werden möglicherweise im Response-Objekt dargestellten abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ab80b-134">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ab80b-135">Alle Eigenschaften werden von einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ab80b-135">All properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



