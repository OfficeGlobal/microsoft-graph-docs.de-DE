---
title: verifyWindowsEnrollmentAutoDiscovery-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cb14317a132d4368a354d8655df56452100bf5a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894299"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="087a0-103">verifyWindowsEnrollmentAutoDiscovery-Funktion</span><span class="sxs-lookup"><span data-stu-id="087a0-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="087a0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="087a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="087a0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="087a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="087a0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="087a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="087a0-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="087a0-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="087a0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="087a0-108">Prerequisites</span></span>
<span data-ttu-id="087a0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="087a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="087a0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="087a0-111">Permission type</span></span>|<span data-ttu-id="087a0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="087a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="087a0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="087a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="087a0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="087a0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="087a0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="087a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="087a0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="087a0-116">Not supported.</span></span>|
|<span data-ttu-id="087a0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="087a0-117">Application</span></span>|<span data-ttu-id="087a0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="087a0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="087a0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="087a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="087a0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="087a0-120">Request headers</span></span>
|<span data-ttu-id="087a0-121">Header</span><span class="sxs-lookup"><span data-stu-id="087a0-121">Header</span></span>|<span data-ttu-id="087a0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="087a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="087a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="087a0-123">Authorization</span></span>|<span data-ttu-id="087a0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="087a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="087a0-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="087a0-125">Accept</span></span>|<span data-ttu-id="087a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="087a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="087a0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="087a0-127">Request body</span></span>
<span data-ttu-id="087a0-128">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="087a0-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="087a0-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="087a0-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="087a0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="087a0-130">Property</span></span>|<span data-ttu-id="087a0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="087a0-131">Type</span></span>|<span data-ttu-id="087a0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="087a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="087a0-133">Domänname</span><span class="sxs-lookup"><span data-stu-id="087a0-133">domainName</span></span>|<span data-ttu-id="087a0-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="087a0-134">String</span></span>|<span data-ttu-id="087a0-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="087a0-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="087a0-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="087a0-136">Response</span></span>
<span data-ttu-id="087a0-137">Wenn die Funktion erfolgreich verläuft, werden der Antwortcode `200 OK` und ein boolescher Wert im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="087a0-137">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="087a0-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="087a0-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="087a0-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="087a0-139">Request</span></span>
<span data-ttu-id="087a0-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="087a0-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="087a0-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="087a0-141">Response</span></span>
<span data-ttu-id="087a0-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="087a0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```





