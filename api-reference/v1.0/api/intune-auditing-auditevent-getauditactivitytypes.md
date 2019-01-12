---
title: Funktion „getAuditActivityTypes“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3a8151169f1173594be3697e721e89556416e718
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952678"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="27f38-103">Funktion „getAuditActivityTypes“</span><span class="sxs-lookup"><span data-stu-id="27f38-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="27f38-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="27f38-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27f38-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="27f38-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27f38-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="27f38-106">Prerequisites</span></span>
<span data-ttu-id="27f38-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27f38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27f38-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="27f38-109">Permission type</span></span>|<span data-ttu-id="27f38-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="27f38-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27f38-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="27f38-111">Delegated (work or school account)</span></span>|<span data-ttu-id="27f38-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="27f38-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="27f38-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="27f38-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27f38-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27f38-114">Not supported.</span></span>|
|<span data-ttu-id="27f38-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="27f38-115">Application</span></span>|<span data-ttu-id="27f38-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="27f38-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27f38-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="27f38-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="27f38-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="27f38-118">Request headers</span></span>
|<span data-ttu-id="27f38-119">Header</span><span class="sxs-lookup"><span data-stu-id="27f38-119">Header</span></span>|<span data-ttu-id="27f38-120">Wert</span><span class="sxs-lookup"><span data-stu-id="27f38-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27f38-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="27f38-121">Authorization</span></span>|<span data-ttu-id="27f38-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="27f38-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27f38-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="27f38-123">Accept</span></span>|<span data-ttu-id="27f38-124">application/json</span><span class="sxs-lookup"><span data-stu-id="27f38-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27f38-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="27f38-125">Request body</span></span>
<span data-ttu-id="27f38-126">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="27f38-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="27f38-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="27f38-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="27f38-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="27f38-128">Property</span></span>|<span data-ttu-id="27f38-129">Typ</span><span class="sxs-lookup"><span data-stu-id="27f38-129">Type</span></span>|<span data-ttu-id="27f38-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="27f38-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27f38-131">Kategorie</span><span class="sxs-lookup"><span data-stu-id="27f38-131">category</span></span>|<span data-ttu-id="27f38-132">String</span><span class="sxs-lookup"><span data-stu-id="27f38-132">String</span></span>|<span data-ttu-id="27f38-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="27f38-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="27f38-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="27f38-134">Response</span></span>
<span data-ttu-id="27f38-135">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="27f38-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27f38-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="27f38-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="27f38-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="27f38-137">Request</span></span>
<span data-ttu-id="27f38-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="27f38-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="27f38-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="27f38-139">Response</span></span>
<span data-ttu-id="27f38-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="27f38-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```



