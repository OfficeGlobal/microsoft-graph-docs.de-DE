---
title: Abrufen von „managedAppStatus“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0d0342d71f10c0353b4a28b23c1440abf5a3f702
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262377"
---
# <a name="get-managedappstatus"></a><span data-ttu-id="4d1c4-103">Abrufen von „managedAppStatus“</span><span class="sxs-lookup"><span data-stu-id="4d1c4-103">Get managedAppStatus</span></span>

> <span data-ttu-id="4d1c4-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4d1c4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d1c4-105">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="4d1c4-105">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d1c4-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4d1c4-106">Prerequisites</span></span>
<span data-ttu-id="4d1c4-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d1c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4d1c4-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d1c4-109">Permission type</span></span>|<span data-ttu-id="4d1c4-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d1c4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d1c4-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d1c4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d1c4-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d1c4-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4d1c4-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d1c4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d1c4-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d1c4-114">Not supported.</span></span>|
|<span data-ttu-id="4d1c4-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d1c4-115">Application</span></span>|<span data-ttu-id="4d1c4-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d1c4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d1c4-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d1c4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d1c4-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4d1c4-118">Optional query parameters</span></span>
<span data-ttu-id="4d1c4-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4d1c4-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d1c4-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d1c4-120">Request headers</span></span>
|<span data-ttu-id="4d1c4-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4d1c4-121">Header</span></span>|<span data-ttu-id="4d1c4-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4d1c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d1c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d1c4-123">Authorization</span></span>|<span data-ttu-id="4d1c4-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d1c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d1c4-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4d1c4-125">Accept</span></span>|<span data-ttu-id="4d1c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d1c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d1c4-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d1c4-127">Request body</span></span>
<span data-ttu-id="4d1c4-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4d1c4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d1c4-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d1c4-129">Response</span></span>
<span data-ttu-id="4d1c4-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppStatus](../resources/intune-mam-managedappstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="4d1c4-130">If successful, this method returns a `200 OK` response code and [managedAppStatus](../resources/intune-mam-managedappstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d1c4-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d1c4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d1c4-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d1c4-132">Request</span></span>
<span data-ttu-id="4d1c4-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d1c4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="4d1c4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d1c4-134">Response</span></span>
<span data-ttu-id="4d1c4-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d1c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



