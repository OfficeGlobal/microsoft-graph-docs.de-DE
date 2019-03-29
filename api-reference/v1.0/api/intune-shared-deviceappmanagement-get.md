---
title: Abrufen von „deviceAppManagement“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 841282551258c23dc57e34c06e803d4184f86809
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958403"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="b6d4d-103">Abrufen von „deviceAppManagement“</span><span class="sxs-lookup"><span data-stu-id="b6d4d-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="b6d4d-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b6d4d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6d4d-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="b6d4d-105">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6d4d-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b6d4d-106">Prerequisites</span></span>

<span data-ttu-id="b6d4d-107">Eine der folgenden Berechtigungen ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="b6d4d-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b6d4d-108">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6d4d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b6d4d-109">Beachten Sie, dass die entsprechende Berechtigung je nach Workflow variiert.</span><span class="sxs-lookup"><span data-stu-id="b6d4d-109">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="b6d4d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b6d4d-110">Permission type</span></span>|<span data-ttu-id="b6d4d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b6d4d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6d4d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b6d4d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6d4d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6d4d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="b6d4d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b6d4d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6d4d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6d4d-115">Not supported.</span></span>|
|<span data-ttu-id="b6d4d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b6d4d-116">Application</span></span>|<span data-ttu-id="b6d4d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6d4d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6d4d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6d4d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b6d4d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b6d4d-119">Optional query parameters</span></span>
<span data-ttu-id="b6d4d-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b6d4d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b6d4d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b6d4d-121">Request headers</span></span>
|<span data-ttu-id="b6d4d-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b6d4d-122">Header</span></span>|<span data-ttu-id="b6d4d-123">Wert</span><span class="sxs-lookup"><span data-stu-id="b6d4d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6d4d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6d4d-124">Authorization</span></span>|<span data-ttu-id="b6d4d-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b6d4d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6d4d-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b6d4d-126">Accept</span></span>|<span data-ttu-id="b6d4d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b6d4d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6d4d-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b6d4d-128">Request body</span></span>
<span data-ttu-id="b6d4d-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b6d4d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6d4d-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6d4d-130">Response</span></span>
<span data-ttu-id="b6d4d-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b6d4d-131">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="b6d4d-132">Beispiel für eine Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6d4d-132">Example request</span></span>

``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement
```

## <a name="example-response"></a><span data-ttu-id="b6d4d-133">Beispielantwort</span><span class="sxs-lookup"><span data-stu-id="b6d4d-133">Example response</span></span>
<span data-ttu-id="b6d4d-134">Das hier gezeigte Antwortobjekt kann zur Kürze abgeschnitten werden.</span><span class="sxs-lookup"><span data-stu-id="b6d4d-134">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b6d4d-135">Alle Eigenschaften werden von einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6d4d-135">All properties will be returned from an actual call.</span></span>

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



