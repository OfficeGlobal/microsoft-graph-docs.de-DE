---
title: Aktion „requestSignupUrl“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 901d0bb67fa5992aa0931afc70660c22cd5ffeca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980041"
---
# <a name="requestsignupurl-action"></a><span data-ttu-id="ff822-103">Aktion „requestSignupUrl“</span><span class="sxs-lookup"><span data-stu-id="ff822-103">requestSignupUrl action</span></span>

> <span data-ttu-id="ff822-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ff822-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff822-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ff822-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff822-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="ff822-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff822-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ff822-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff822-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ff822-108">Prerequisites</span></span>
<span data-ttu-id="ff822-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff822-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff822-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ff822-111">Permission type</span></span>|<span data-ttu-id="ff822-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ff822-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff822-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ff822-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff822-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff822-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ff822-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ff822-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff822-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff822-116">Not supported.</span></span>|
|<span data-ttu-id="ff822-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ff822-117">Application</span></span>|<span data-ttu-id="ff822-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ff822-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff822-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff822-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkSettings/requestSignupUrl
```

## <a name="request-headers"></a><span data-ttu-id="ff822-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ff822-120">Request headers</span></span>
|<span data-ttu-id="ff822-121">Header</span><span class="sxs-lookup"><span data-stu-id="ff822-121">Header</span></span>|<span data-ttu-id="ff822-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ff822-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff822-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff822-123">Authorization</span></span>|<span data-ttu-id="ff822-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ff822-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff822-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ff822-125">Accept</span></span>|<span data-ttu-id="ff822-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff822-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff822-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ff822-127">Request body</span></span>
<span data-ttu-id="ff822-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="ff822-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ff822-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="ff822-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ff822-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ff822-130">Property</span></span>|<span data-ttu-id="ff822-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ff822-131">Type</span></span>|<span data-ttu-id="ff822-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ff822-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff822-133">hostName</span><span class="sxs-lookup"><span data-stu-id="ff822-133">hostName</span></span>|<span data-ttu-id="ff822-134">String</span><span class="sxs-lookup"><span data-stu-id="ff822-134">String</span></span>|<span data-ttu-id="ff822-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ff822-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ff822-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff822-136">Response</span></span>
<span data-ttu-id="ff822-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `200 OK` und ein Objekt des Typs „String“ im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ff822-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff822-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ff822-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff822-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ff822-139">Request</span></span>
<span data-ttu-id="ff822-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ff822-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings/requestSignupUrl

Content-type: application/json
Content-length: 37

{
  "hostName": "Host Name value"
}
```

### <a name="response"></a><span data-ttu-id="ff822-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="ff822-141">Response</span></span>
<span data-ttu-id="ff822-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ff822-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": "https://example.com/requestSignupUrl/"
}
```





