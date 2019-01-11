---
title: Aktion „createToken“
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a7c39af9c77728e2ccfbc5bc4412058a3b0b8fc2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892386"
---
# <a name="createtoken-action"></a><span data-ttu-id="2a967-103">Aktion „createToken“</span><span class="sxs-lookup"><span data-stu-id="2a967-103">createToken action</span></span>

> <span data-ttu-id="2a967-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2a967-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2a967-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2a967-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a967-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="2a967-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a967-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2a967-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a967-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="2a967-108">Prerequisites</span></span>
<span data-ttu-id="2a967-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a967-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a967-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a967-111">Permission type</span></span>|<span data-ttu-id="2a967-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a967-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a967-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a967-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a967-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a967-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a967-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a967-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a967-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a967-116">Not supported.</span></span>|
|<span data-ttu-id="2a967-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a967-117">Application</span></span>|<span data-ttu-id="2a967-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a967-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a967-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a967-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/createToken
```

## <a name="request-headers"></a><span data-ttu-id="2a967-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a967-120">Request headers</span></span>
|<span data-ttu-id="2a967-121">Header</span><span class="sxs-lookup"><span data-stu-id="2a967-121">Header</span></span>|<span data-ttu-id="2a967-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2a967-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a967-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a967-123">Authorization</span></span>|<span data-ttu-id="2a967-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="2a967-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a967-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2a967-125">Accept</span></span>|<span data-ttu-id="2a967-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a967-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a967-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a967-127">Request body</span></span>
<span data-ttu-id="2a967-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="2a967-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2a967-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="2a967-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2a967-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2a967-130">Property</span></span>|<span data-ttu-id="2a967-131">Typ</span><span class="sxs-lookup"><span data-stu-id="2a967-131">Type</span></span>|<span data-ttu-id="2a967-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a967-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a967-133">tokenValidityInSeconds</span><span class="sxs-lookup"><span data-stu-id="2a967-133">tokenValidityInSeconds</span></span>|<span data-ttu-id="2a967-134">Int32</span><span class="sxs-lookup"><span data-stu-id="2a967-134">Int32</span></span>|<span data-ttu-id="2a967-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="2a967-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2a967-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a967-136">Response</span></span>
<span data-ttu-id="2a967-137">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="2a967-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2a967-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a967-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a967-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a967-139">Request</span></span>
<span data-ttu-id="2a967-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a967-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}/createToken

Content-type: application/json
Content-length: 35

{
  "tokenValidityInSeconds": 6
}
```

### <a name="response"></a><span data-ttu-id="2a967-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a967-141">Response</span></span>
<span data-ttu-id="2a967-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a967-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





