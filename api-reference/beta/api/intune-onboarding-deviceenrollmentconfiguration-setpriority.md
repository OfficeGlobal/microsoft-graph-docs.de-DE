---
title: setPriority-Aktion
description: Noch nicht dokumentiert
ms.openlocfilehash: d041c5c27d3ae0a83839a50bb8b841f570a81cbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065728"
---
# <a name="setpriority-action"></a><span data-ttu-id="3b4a2-103">setPriority-Aktion</span><span class="sxs-lookup"><span data-stu-id="3b4a2-103">setPriority action</span></span>

> <span data-ttu-id="3b4a2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b4a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b4a2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b4a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b4a2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3b4a2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b4a2-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3b4a2-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b4a2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3b4a2-108">Prerequisites</span></span>
<span data-ttu-id="3b4a2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b4a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b4a2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3b4a2-111">Permission type</span></span>|<span data-ttu-id="3b4a2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3b4a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b4a2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3b4a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b4a2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b4a2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3b4a2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3b4a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b4a2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b4a2-116">Not supported.</span></span>|
|<span data-ttu-id="3b4a2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3b4a2-117">Application</span></span>|<span data-ttu-id="3b4a2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3b4a2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b4a2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b4a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="3b4a2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b4a2-120">Request headers</span></span>
|<span data-ttu-id="3b4a2-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3b4a2-121">Header</span></span>|<span data-ttu-id="3b4a2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3b4a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b4a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b4a2-123">Authorization</span></span>|<span data-ttu-id="3b4a2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="3b4a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b4a2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b4a2-125">Accept</span></span>|<span data-ttu-id="3b4a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b4a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b4a2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b4a2-127">Request body</span></span>
<span data-ttu-id="3b4a2-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="3b4a2-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3b4a2-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="3b4a2-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3b4a2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b4a2-130">Property</span></span>|<span data-ttu-id="3b4a2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="3b4a2-131">Type</span></span>|<span data-ttu-id="3b4a2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b4a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b4a2-133">Priorität</span><span class="sxs-lookup"><span data-stu-id="3b4a2-133">priority</span></span>|<span data-ttu-id="3b4a2-134">Int32</span><span class="sxs-lookup"><span data-stu-id="3b4a2-134">Int32</span></span>|<span data-ttu-id="3b4a2-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3b4a2-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3b4a2-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b4a2-136">Response</span></span>
<span data-ttu-id="3b4a2-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="3b4a2-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3b4a2-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3b4a2-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b4a2-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b4a2-139">Request</span></span>
<span data-ttu-id="3b4a2-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3b4a2-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="3b4a2-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b4a2-141">Response</span></span>
<span data-ttu-id="3b4a2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3b4a2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





