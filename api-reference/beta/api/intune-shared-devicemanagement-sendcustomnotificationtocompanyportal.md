---
title: SendCustomNotificationToCompanyPortal Aktion
description: Noch nicht dokumentiert
ms.openlocfilehash: bf19f87c385568a38407fff0df144c6df165fbc0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060718"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="b1580-103">SendCustomNotificationToCompanyPortal Aktion</span><span class="sxs-lookup"><span data-stu-id="b1580-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="b1580-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b1580-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1580-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1580-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1580-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b1580-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1580-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b1580-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b1580-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b1580-108">Prerequisites</span></span>
<span data-ttu-id="b1580-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1580-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1580-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b1580-111">Permission type</span></span>|<span data-ttu-id="b1580-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b1580-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1580-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b1580-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b1580-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="b1580-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b1580-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1580-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b1580-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b1580-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1580-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1580-117">Not supported.</span></span>|
|<span data-ttu-id="b1580-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b1580-118">Application</span></span>|<span data-ttu-id="b1580-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b1580-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1580-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1580-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="b1580-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b1580-121">Request headers</span></span>
|<span data-ttu-id="b1580-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b1580-122">Header</span></span>|<span data-ttu-id="b1580-123">Wert</span><span class="sxs-lookup"><span data-stu-id="b1580-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1580-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1580-124">Authorization</span></span>|<span data-ttu-id="b1580-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b1580-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1580-126">Accept</span><span class="sxs-lookup"><span data-stu-id="b1580-126">Accept</span></span>|<span data-ttu-id="b1580-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b1580-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1580-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b1580-128">Request body</span></span>
<span data-ttu-id="b1580-129">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="b1580-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b1580-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="b1580-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b1580-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b1580-131">Property</span></span>|<span data-ttu-id="b1580-132">Typ</span><span class="sxs-lookup"><span data-stu-id="b1580-132">Type</span></span>|<span data-ttu-id="b1580-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1580-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1580-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="b1580-134">notificationTitle</span></span>|<span data-ttu-id="b1580-135">String</span><span class="sxs-lookup"><span data-stu-id="b1580-135">String</span></span>|<span data-ttu-id="b1580-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b1580-136">Not yet documented</span></span>|
|<span data-ttu-id="b1580-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="b1580-137">notificationBody</span></span>|<span data-ttu-id="b1580-138">String</span><span class="sxs-lookup"><span data-stu-id="b1580-138">String</span></span>|<span data-ttu-id="b1580-139">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b1580-139">Not yet documented</span></span>|
|<span data-ttu-id="b1580-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="b1580-140">groupsToNotify</span></span>|<span data-ttu-id="b1580-141">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b1580-141">String collection</span></span>|<span data-ttu-id="b1580-142">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="b1580-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b1580-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1580-143">Response</span></span>
<span data-ttu-id="b1580-144">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="b1580-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b1580-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b1580-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1580-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b1580-146">Request</span></span>
<span data-ttu-id="b1580-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b1580-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1580-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="b1580-148">Response</span></span>
<span data-ttu-id="b1580-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b1580-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






