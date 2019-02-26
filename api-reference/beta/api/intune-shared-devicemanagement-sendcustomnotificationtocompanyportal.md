---
title: sendCustomNotificationToCompanyPortal-Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c204a48d7b55f930e3eee4ec017843d8ff59ccc2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162272"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="c630c-103">sendCustomNotificationToCompanyPortal-Aktion</span><span class="sxs-lookup"><span data-stu-id="c630c-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="c630c-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="c630c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c630c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c630c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c630c-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c630c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c630c-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c630c-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c630c-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c630c-108">Prerequisites</span></span>
<span data-ttu-id="c630c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c630c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="c630c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c630c-111">Permission type</span></span>|<span data-ttu-id="c630c-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c630c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c630c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c630c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c630c-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="c630c-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c630c-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c630c-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c630c-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c630c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c630c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c630c-117">Not supported.</span></span>|
|<span data-ttu-id="c630c-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c630c-118">Application</span></span>|<span data-ttu-id="c630c-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c630c-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c630c-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c630c-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="c630c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c630c-121">Request headers</span></span>
|<span data-ttu-id="c630c-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c630c-122">Header</span></span>|<span data-ttu-id="c630c-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c630c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c630c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c630c-124">Authorization</span></span>|<span data-ttu-id="c630c-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c630c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c630c-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c630c-126">Accept</span></span>|<span data-ttu-id="c630c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c630c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c630c-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c630c-128">Request body</span></span>
<span data-ttu-id="c630c-129">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="c630c-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c630c-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="c630c-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c630c-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c630c-131">Property</span></span>|<span data-ttu-id="c630c-132">Typ</span><span class="sxs-lookup"><span data-stu-id="c630c-132">Type</span></span>|<span data-ttu-id="c630c-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c630c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c630c-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="c630c-134">notificationTitle</span></span>|<span data-ttu-id="c630c-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c630c-135">String</span></span>|<span data-ttu-id="c630c-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c630c-136">Not yet documented</span></span>|
|<span data-ttu-id="c630c-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="c630c-137">notificationBody</span></span>|<span data-ttu-id="c630c-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c630c-138">String</span></span>|<span data-ttu-id="c630c-139">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="c630c-139">Not yet documented</span></span>|
|<span data-ttu-id="c630c-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="c630c-140">groupsToNotify</span></span>|<span data-ttu-id="c630c-141">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="c630c-141">String collection</span></span>|<span data-ttu-id="c630c-142">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="c630c-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c630c-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="c630c-143">Response</span></span>
<span data-ttu-id="c630c-144">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="c630c-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c630c-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c630c-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="c630c-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c630c-146">Request</span></span>
<span data-ttu-id="c630c-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c630c-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c630c-148">Reaktion</span><span class="sxs-lookup"><span data-stu-id="c630c-148">Response</span></span>
<span data-ttu-id="c630c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c630c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






