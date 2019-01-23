---
title: GetScopesForUser-Funktion
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 383e4cf835b8f056af707367b3664e0bac4a59a1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396168"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="c5a40-103">GetScopesForUser-Funktion</span><span class="sxs-lookup"><span data-stu-id="c5a40-103">getScopesForUser function</span></span>

> <span data-ttu-id="c5a40-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c5a40-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c5a40-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c5a40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5a40-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c5a40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5a40-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c5a40-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5a40-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c5a40-108">Prerequisites</span></span>
<span data-ttu-id="c5a40-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c5a40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c5a40-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c5a40-111">Permission type</span></span>|<span data-ttu-id="c5a40-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c5a40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5a40-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c5a40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5a40-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5a40-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="c5a40-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c5a40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5a40-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5a40-116">Not supported.</span></span>|
|<span data-ttu-id="c5a40-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c5a40-117">Application</span></span>|<span data-ttu-id="c5a40-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c5a40-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5a40-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5a40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="c5a40-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c5a40-120">Request headers</span></span>
|<span data-ttu-id="c5a40-121">Header</span><span class="sxs-lookup"><span data-stu-id="c5a40-121">Header</span></span>|<span data-ttu-id="c5a40-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c5a40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5a40-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c5a40-123">Authorization</span></span>|<span data-ttu-id="c5a40-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c5a40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5a40-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c5a40-125">Accept</span></span>|<span data-ttu-id="c5a40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5a40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5a40-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c5a40-127">Request body</span></span>
<span data-ttu-id="c5a40-128">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="c5a40-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="c5a40-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="c5a40-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c5a40-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c5a40-130">Property</span></span>|<span data-ttu-id="c5a40-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c5a40-131">Type</span></span>|<span data-ttu-id="c5a40-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c5a40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a40-133">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="c5a40-133">userid</span></span>|<span data-ttu-id="c5a40-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c5a40-134">String</span></span>|<span data-ttu-id="c5a40-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c5a40-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c5a40-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5a40-136">Response</span></span>
<span data-ttu-id="c5a40-137">Bei erfolgreicher Ausführung gibt die Funktion den Antwortcode `200 OK` und eine Collection von Objekten des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c5a40-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5a40-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c5a40-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5a40-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c5a40-139">Request</span></span>
<span data-ttu-id="c5a40-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c5a40-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="c5a40-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="c5a40-141">Response</span></span>
<span data-ttu-id="c5a40-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c5a40-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": [
    "Get Scopes For User value"
  ]
}
```




