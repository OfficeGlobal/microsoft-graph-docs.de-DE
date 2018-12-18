---
title: verifyWindowsEnrollmentAutoDiscovery-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 3f981ae765981c067b08dc08dae96831f59d572b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344177"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="5f740-103">verifyWindowsEnrollmentAutoDiscovery-Funktion</span><span class="sxs-lookup"><span data-stu-id="5f740-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="5f740-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="5f740-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f740-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5f740-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f740-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5f740-106">Prerequisites</span></span>
<span data-ttu-id="5f740-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f740-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f740-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f740-109">Permission type</span></span>|<span data-ttu-id="5f740-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f740-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f740-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f740-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5f740-112">&nbsp;&nbsp; Onboarding</span><span class="sxs-lookup"><span data-stu-id="5f740-112">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="5f740-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f740-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5f740-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f740-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f740-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f740-115">Not supported.</span></span>|
|<span data-ttu-id="5f740-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f740-116">Application</span></span>|<span data-ttu-id="5f740-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f740-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f740-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f740-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="5f740-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f740-119">Request headers</span></span>
|<span data-ttu-id="5f740-120">Header</span><span class="sxs-lookup"><span data-stu-id="5f740-120">Header</span></span>|<span data-ttu-id="5f740-121">Wert</span><span class="sxs-lookup"><span data-stu-id="5f740-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f740-122">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5f740-122">Authorization</span></span>|<span data-ttu-id="5f740-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5f740-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f740-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5f740-124">Accept</span></span>|<span data-ttu-id="5f740-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5f740-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f740-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f740-126">Request body</span></span>
<span data-ttu-id="5f740-127">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="5f740-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="5f740-128">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="5f740-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="5f740-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5f740-129">Property</span></span>|<span data-ttu-id="5f740-130">Typ</span><span class="sxs-lookup"><span data-stu-id="5f740-130">Type</span></span>|<span data-ttu-id="5f740-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f740-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f740-132">Domänname</span><span class="sxs-lookup"><span data-stu-id="5f740-132">domainName</span></span>|<span data-ttu-id="5f740-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="5f740-133">String</span></span>|<span data-ttu-id="5f740-134">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="5f740-134">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="5f740-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f740-135">Response</span></span>
<span data-ttu-id="5f740-136">Wenn die Funktion erfolgreich verläuft, werden der Antwortcode `200 OK` und ein boolescher Wert im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f740-136">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f740-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f740-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f740-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f740-138">Request</span></span>
<span data-ttu-id="5f740-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5f740-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="5f740-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f740-140">Response</span></span>
<span data-ttu-id="5f740-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f740-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



