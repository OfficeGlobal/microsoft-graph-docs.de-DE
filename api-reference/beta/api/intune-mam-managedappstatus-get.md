---
title: Abrufen von „managedAppStatus“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs managedAppStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 085c9cc0bf5445c039462e92f870b264ae5bec4b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419149"
---
# <a name="get-managedappstatus"></a><span data-ttu-id="3a38d-103">Abrufen von „managedAppStatus“</span><span class="sxs-lookup"><span data-stu-id="3a38d-103">Get managedAppStatus</span></span>

> <span data-ttu-id="3a38d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="3a38d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3a38d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3a38d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3a38d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a38d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a38d-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="3a38d-107">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a38d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3a38d-108">Prerequisites</span></span>
<span data-ttu-id="3a38d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3a38d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3a38d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a38d-111">Permission type</span></span>|<span data-ttu-id="3a38d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a38d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a38d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a38d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a38d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3a38d-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3a38d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a38d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a38d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a38d-116">Not supported.</span></span>|
|<span data-ttu-id="3a38d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a38d-117">Application</span></span>|<span data-ttu-id="3a38d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a38d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a38d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a38d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a38d-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3a38d-120">Optional query parameters</span></span>
<span data-ttu-id="3a38d-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3a38d-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a38d-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a38d-122">Request headers</span></span>
|<span data-ttu-id="3a38d-123">Header</span><span class="sxs-lookup"><span data-stu-id="3a38d-123">Header</span></span>|<span data-ttu-id="3a38d-124">Wert</span><span class="sxs-lookup"><span data-stu-id="3a38d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a38d-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="3a38d-125">Authorization</span></span>|<span data-ttu-id="3a38d-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3a38d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a38d-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3a38d-127">Accept</span></span>|<span data-ttu-id="3a38d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3a38d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a38d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a38d-129">Request body</span></span>
<span data-ttu-id="3a38d-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3a38d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a38d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a38d-131">Response</span></span>
<span data-ttu-id="3a38d-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [managedAppStatus](../resources/intune-mam-managedappstatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="3a38d-132">If successful, this method returns a `200 OK` response code and [managedAppStatus](../resources/intune-mam-managedappstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a38d-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a38d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a38d-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a38d-134">Request</span></span>
<span data-ttu-id="3a38d-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a38d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

### <a name="response"></a><span data-ttu-id="3a38d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a38d-136">Response</span></span>
<span data-ttu-id="3a38d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a38d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




