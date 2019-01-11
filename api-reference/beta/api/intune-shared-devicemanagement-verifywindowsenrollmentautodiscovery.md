---
title: verifyWindowsEnrollmentAutoDiscovery-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 144fb484a9d372c2f3173b300274901c9fdc3dd1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823660"
---
# <a name="verifywindowsenrollmentautodiscovery-function"></a><span data-ttu-id="516aa-103">verifyWindowsEnrollmentAutoDiscovery-Funktion</span><span class="sxs-lookup"><span data-stu-id="516aa-103">verifyWindowsEnrollmentAutoDiscovery function</span></span>

> <span data-ttu-id="516aa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="516aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="516aa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="516aa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="516aa-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="516aa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="516aa-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="516aa-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="516aa-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="516aa-108">Prerequisites</span></span>
<span data-ttu-id="516aa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="516aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="516aa-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="516aa-111">Permission type</span></span>|<span data-ttu-id="516aa-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="516aa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="516aa-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="516aa-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="516aa-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="516aa-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="516aa-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="516aa-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="516aa-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="516aa-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="516aa-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="516aa-117">Not supported.</span></span>|
|<span data-ttu-id="516aa-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="516aa-118">Application</span></span>|<span data-ttu-id="516aa-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="516aa-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="516aa-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="516aa-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/verifyWindowsEnrollmentAutoDiscovery
```

## <a name="request-headers"></a><span data-ttu-id="516aa-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="516aa-121">Request headers</span></span>
|<span data-ttu-id="516aa-122">Header</span><span class="sxs-lookup"><span data-stu-id="516aa-122">Header</span></span>|<span data-ttu-id="516aa-123">Wert</span><span class="sxs-lookup"><span data-stu-id="516aa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="516aa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="516aa-124">Authorization</span></span>|<span data-ttu-id="516aa-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="516aa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="516aa-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="516aa-126">Accept</span></span>|<span data-ttu-id="516aa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="516aa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="516aa-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="516aa-128">Request body</span></span>
<span data-ttu-id="516aa-129">Geben Sie in der Anforderungs-URL die folgenden Abfrageparameter mit Werten an.</span><span class="sxs-lookup"><span data-stu-id="516aa-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="516aa-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="516aa-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="516aa-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="516aa-131">Property</span></span>|<span data-ttu-id="516aa-132">Typ</span><span class="sxs-lookup"><span data-stu-id="516aa-132">Type</span></span>|<span data-ttu-id="516aa-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="516aa-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="516aa-134">Domänname</span><span class="sxs-lookup"><span data-stu-id="516aa-134">domainName</span></span>|<span data-ttu-id="516aa-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="516aa-135">String</span></span>|<span data-ttu-id="516aa-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="516aa-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="516aa-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="516aa-137">Response</span></span>
<span data-ttu-id="516aa-138">Wenn die Funktion erfolgreich verläuft, werden der Antwortcode `200 OK` und ein boolescher Wert im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="516aa-138">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="516aa-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="516aa-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="516aa-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="516aa-140">Request</span></span>
<span data-ttu-id="516aa-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="516aa-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/verifyWindowsEnrollmentAutoDiscovery(domainName='parameterValue')
```

### <a name="response"></a><span data-ttu-id="516aa-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="516aa-142">Response</span></span>
<span data-ttu-id="516aa-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="516aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```



