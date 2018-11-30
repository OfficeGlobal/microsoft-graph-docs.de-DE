---
title: Aktion „requestSignupUrl“
description: Noch nicht dokumentiert
ms.openlocfilehash: d4d6084de274ccf9cf8bdf64fd198ef353e27f54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064511"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="7b452-103">Aktion „requestSignupUrl“</span><span class="sxs-lookup"><span data-stu-id="7b452-103">requestSignupUrl action</span></span>

> <span data-ttu-id="7b452-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7b452-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b452-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7b452-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b452-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="7b452-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7b452-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7b452-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b452-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7b452-108">Prerequisites</span></span>
<span data-ttu-id="7b452-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b452-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b452-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b452-111">Permission type</span></span>|<span data-ttu-id="7b452-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b452-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b452-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b452-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b452-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b452-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7b452-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b452-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b452-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b452-116">Not supported.</span></span>|
|<span data-ttu-id="7b452-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b452-117">Application</span></span>|<span data-ttu-id="7b452-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b452-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b452-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b452-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="7b452-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b452-120">Request headers</span></span>
|<span data-ttu-id="7b452-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7b452-121">Header</span></span>|<span data-ttu-id="7b452-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7b452-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b452-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b452-123">Authorization</span></span>|<span data-ttu-id="7b452-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7b452-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b452-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7b452-125">Accept</span></span>|<span data-ttu-id="7b452-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b452-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b452-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b452-127">Request body</span></span>
<span data-ttu-id="7b452-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="7b452-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7b452-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="7b452-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7b452-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7b452-130">Property</span></span>|<span data-ttu-id="7b452-131">Typ</span><span class="sxs-lookup"><span data-stu-id="7b452-131">Type</span></span>|<span data-ttu-id="7b452-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b452-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b452-133">hostName</span><span class="sxs-lookup"><span data-stu-id="7b452-133">hostName</span></span>|<span data-ttu-id="7b452-134">String</span><span class="sxs-lookup"><span data-stu-id="7b452-134">String</span></span>|<span data-ttu-id="7b452-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="7b452-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7b452-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b452-136">Response</span></span>
<span data-ttu-id="7b452-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7b452-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b452-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b452-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="7b452-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b452-139">Request</span></span>
<span data-ttu-id="7b452-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b452-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="7b452-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b452-141">Response</span></span>
<span data-ttu-id="7b452-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b452-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```





