---
title: SendCustomNotificationToCompanyPortal Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b5a3e4acedb95fe1092a6ef9eaacc2978fedcd9b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851163"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="fd4cb-103">SendCustomNotificationToCompanyPortal Aktion</span><span class="sxs-lookup"><span data-stu-id="fd4cb-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="fd4cb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fd4cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd4cb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fd4cb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd4cb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fd4cb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd4cb-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fd4cb-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd4cb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fd4cb-108">Prerequisites</span></span>
<span data-ttu-id="fd4cb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd4cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd4cb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd4cb-111">Permission type</span></span>|<span data-ttu-id="fd4cb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd4cb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd4cb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd4cb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fd4cb-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="fd4cb-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fd4cb-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd4cb-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fd4cb-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd4cb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd4cb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd4cb-117">Not supported.</span></span>|
|<span data-ttu-id="fd4cb-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd4cb-118">Application</span></span>|<span data-ttu-id="fd4cb-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd4cb-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd4cb-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd4cb-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="fd4cb-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd4cb-121">Request headers</span></span>
|<span data-ttu-id="fd4cb-122">Header</span><span class="sxs-lookup"><span data-stu-id="fd4cb-122">Header</span></span>|<span data-ttu-id="fd4cb-123">Wert</span><span class="sxs-lookup"><span data-stu-id="fd4cb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd4cb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd4cb-124">Authorization</span></span>|<span data-ttu-id="fd4cb-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fd4cb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd4cb-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fd4cb-126">Accept</span></span>|<span data-ttu-id="fd4cb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fd4cb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd4cb-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd4cb-128">Request body</span></span>
<span data-ttu-id="fd4cb-129">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="fd4cb-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fd4cb-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="fd4cb-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fd4cb-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fd4cb-131">Property</span></span>|<span data-ttu-id="fd4cb-132">Typ</span><span class="sxs-lookup"><span data-stu-id="fd4cb-132">Type</span></span>|<span data-ttu-id="fd4cb-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd4cb-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd4cb-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="fd4cb-134">notificationTitle</span></span>|<span data-ttu-id="fd4cb-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fd4cb-135">String</span></span>|<span data-ttu-id="fd4cb-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fd4cb-136">Not yet documented</span></span>|
|<span data-ttu-id="fd4cb-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="fd4cb-137">notificationBody</span></span>|<span data-ttu-id="fd4cb-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fd4cb-138">String</span></span>|<span data-ttu-id="fd4cb-139">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fd4cb-139">Not yet documented</span></span>|
|<span data-ttu-id="fd4cb-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="fd4cb-140">groupsToNotify</span></span>|<span data-ttu-id="fd4cb-141">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="fd4cb-141">String collection</span></span>|<span data-ttu-id="fd4cb-142">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fd4cb-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fd4cb-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd4cb-143">Response</span></span>
<span data-ttu-id="fd4cb-144">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="fd4cb-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fd4cb-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd4cb-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd4cb-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd4cb-146">Request</span></span>
<span data-ttu-id="fd4cb-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd4cb-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/sendCustomNotificationToCompanyPortal

Content-type: application/json
Content-length: 164

{
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value",
  "groupsToNotify": [
    "Groups To Notify value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="fd4cb-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd4cb-148">Response</span></span>
<span data-ttu-id="fd4cb-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd4cb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






