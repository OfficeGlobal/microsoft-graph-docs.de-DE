---
title: setPriority-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 405c7094e0513d5162eb2120a73892904dbf8b6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954736"
---
# <a name="setpriority-action"></a><span data-ttu-id="c9128-103">setPriority-Aktion</span><span class="sxs-lookup"><span data-stu-id="c9128-103">setPriority action</span></span>

> <span data-ttu-id="c9128-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c9128-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9128-105">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c9128-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9128-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c9128-106">Prerequisites</span></span>
<span data-ttu-id="c9128-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9128-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9128-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9128-109">Permission type</span></span>|<span data-ttu-id="c9128-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9128-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9128-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9128-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c9128-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9128-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c9128-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9128-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9128-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9128-114">Not supported.</span></span>|
|<span data-ttu-id="c9128-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9128-115">Application</span></span>|<span data-ttu-id="c9128-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c9128-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9128-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9128-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority
```

## <a name="request-headers"></a><span data-ttu-id="c9128-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9128-118">Request headers</span></span>
|<span data-ttu-id="c9128-119">Header</span><span class="sxs-lookup"><span data-stu-id="c9128-119">Header</span></span>|<span data-ttu-id="c9128-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c9128-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9128-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9128-121">Authorization</span></span>|<span data-ttu-id="c9128-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c9128-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9128-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c9128-123">Accept</span></span>|<span data-ttu-id="c9128-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c9128-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9128-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9128-125">Request body</span></span>
<span data-ttu-id="c9128-126">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="c9128-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c9128-127">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="c9128-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c9128-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9128-128">Property</span></span>|<span data-ttu-id="c9128-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c9128-129">Type</span></span>|<span data-ttu-id="c9128-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9128-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9128-131">Priorität</span><span class="sxs-lookup"><span data-stu-id="c9128-131">priority</span></span>|<span data-ttu-id="c9128-132">Int32</span><span class="sxs-lookup"><span data-stu-id="c9128-132">Int32</span></span>|<span data-ttu-id="c9128-133">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c9128-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c9128-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9128-134">Response</span></span>
<span data-ttu-id="c9128-135">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="c9128-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c9128-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9128-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="c9128-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9128-137">Request</span></span>
<span data-ttu-id="c9128-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9128-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/setPriority

Content-type: application/json
Content-length: 21

{
  "priority": 8
}
```

### <a name="response"></a><span data-ttu-id="c9128-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9128-139">Response</span></span>
<span data-ttu-id="c9128-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9128-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



