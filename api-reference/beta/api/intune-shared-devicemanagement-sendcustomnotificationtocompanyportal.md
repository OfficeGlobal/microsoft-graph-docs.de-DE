---
title: SendCustomNotificationToCompanyPortal Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7314f833fb5e11cdbf447b748a12634210c4d6f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940512"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="56f06-103">SendCustomNotificationToCompanyPortal Aktion</span><span class="sxs-lookup"><span data-stu-id="56f06-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="56f06-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="56f06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56f06-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56f06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56f06-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="56f06-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56f06-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="56f06-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56f06-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="56f06-108">Prerequisites</span></span>
<span data-ttu-id="56f06-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56f06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56f06-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56f06-111">Permission type</span></span>|<span data-ttu-id="56f06-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56f06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56f06-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56f06-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="56f06-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="56f06-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="56f06-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56f06-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="56f06-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56f06-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56f06-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56f06-117">Not supported.</span></span>|
|<span data-ttu-id="56f06-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56f06-118">Application</span></span>|<span data-ttu-id="56f06-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56f06-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56f06-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56f06-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="56f06-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56f06-121">Request headers</span></span>
|<span data-ttu-id="56f06-122">Header</span><span class="sxs-lookup"><span data-stu-id="56f06-122">Header</span></span>|<span data-ttu-id="56f06-123">Wert</span><span class="sxs-lookup"><span data-stu-id="56f06-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56f06-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="56f06-124">Authorization</span></span>|<span data-ttu-id="56f06-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="56f06-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56f06-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="56f06-126">Accept</span></span>|<span data-ttu-id="56f06-127">application/json</span><span class="sxs-lookup"><span data-stu-id="56f06-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56f06-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56f06-128">Request body</span></span>
<span data-ttu-id="56f06-129">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="56f06-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="56f06-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="56f06-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="56f06-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="56f06-131">Property</span></span>|<span data-ttu-id="56f06-132">Typ</span><span class="sxs-lookup"><span data-stu-id="56f06-132">Type</span></span>|<span data-ttu-id="56f06-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56f06-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56f06-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="56f06-134">notificationTitle</span></span>|<span data-ttu-id="56f06-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56f06-135">String</span></span>|<span data-ttu-id="56f06-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="56f06-136">Not yet documented</span></span>|
|<span data-ttu-id="56f06-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="56f06-137">notificationBody</span></span>|<span data-ttu-id="56f06-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="56f06-138">String</span></span>|<span data-ttu-id="56f06-139">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="56f06-139">Not yet documented</span></span>|
|<span data-ttu-id="56f06-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="56f06-140">groupsToNotify</span></span>|<span data-ttu-id="56f06-141">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="56f06-141">String collection</span></span>|<span data-ttu-id="56f06-142">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="56f06-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="56f06-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="56f06-143">Response</span></span>
<span data-ttu-id="56f06-144">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="56f06-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="56f06-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56f06-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="56f06-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56f06-146">Request</span></span>
<span data-ttu-id="56f06-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56f06-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="56f06-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="56f06-148">Response</span></span>
<span data-ttu-id="56f06-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56f06-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






