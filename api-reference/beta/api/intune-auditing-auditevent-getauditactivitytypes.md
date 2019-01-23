---
title: Funktion „getAuditActivityTypes“
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a5a5ee1341eea12024c9de03a111ee781ac2c184
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401768"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="24467-103">Funktion „getAuditActivityTypes“</span><span class="sxs-lookup"><span data-stu-id="24467-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="24467-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="24467-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="24467-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24467-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24467-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24467-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24467-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="24467-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24467-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="24467-108">Prerequisites</span></span>
<span data-ttu-id="24467-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="24467-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="24467-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="24467-111">Permission type</span></span>|<span data-ttu-id="24467-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="24467-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24467-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="24467-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24467-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="24467-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="24467-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="24467-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24467-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24467-116">Not supported.</span></span>|
|<span data-ttu-id="24467-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="24467-117">Application</span></span>|<span data-ttu-id="24467-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="24467-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24467-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="24467-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="24467-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="24467-120">Request headers</span></span>
|<span data-ttu-id="24467-121">Header</span><span class="sxs-lookup"><span data-stu-id="24467-121">Header</span></span>|<span data-ttu-id="24467-122">Wert</span><span class="sxs-lookup"><span data-stu-id="24467-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24467-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="24467-123">Authorization</span></span>|<span data-ttu-id="24467-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="24467-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24467-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="24467-125">Accept</span></span>|<span data-ttu-id="24467-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24467-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24467-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="24467-127">Request body</span></span>
<span data-ttu-id="24467-128">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="24467-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="24467-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="24467-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="24467-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="24467-130">Property</span></span>|<span data-ttu-id="24467-131">Typ</span><span class="sxs-lookup"><span data-stu-id="24467-131">Type</span></span>|<span data-ttu-id="24467-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24467-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24467-133">Kategorie</span><span class="sxs-lookup"><span data-stu-id="24467-133">category</span></span>|<span data-ttu-id="24467-134">String</span><span class="sxs-lookup"><span data-stu-id="24467-134">String</span></span>|<span data-ttu-id="24467-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="24467-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="24467-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="24467-136">Response</span></span>
<span data-ttu-id="24467-137">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="24467-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24467-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="24467-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="24467-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="24467-139">Request</span></span>
<span data-ttu-id="24467-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="24467-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="24467-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="24467-141">Response</span></span>
<span data-ttu-id="24467-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="24467-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




