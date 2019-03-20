---
title: sendCustomNotificationToCompanyPortal-Aktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e27ef7874813247772e26d33dcd31fc80ffba623
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572495"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="bb856-103">sendCustomNotificationToCompanyPortal-Aktion</span><span class="sxs-lookup"><span data-stu-id="bb856-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="bb856-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="bb856-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bb856-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bb856-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb856-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bb856-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb856-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bb856-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb856-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bb856-108">Prerequisites</span></span>
<span data-ttu-id="bb856-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bb856-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bb856-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bb856-111">Permission type</span></span>|<span data-ttu-id="bb856-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bb856-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb856-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bb856-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bb856-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="bb856-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="bb856-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb856-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bb856-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bb856-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb856-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb856-117">Not supported.</span></span>|
|<span data-ttu-id="bb856-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bb856-118">Application</span></span>|<span data-ttu-id="bb856-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bb856-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb856-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb856-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="bb856-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bb856-121">Request headers</span></span>
|<span data-ttu-id="bb856-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bb856-122">Header</span></span>|<span data-ttu-id="bb856-123">Wert</span><span class="sxs-lookup"><span data-stu-id="bb856-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb856-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb856-124">Authorization</span></span>|<span data-ttu-id="bb856-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bb856-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb856-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bb856-126">Accept</span></span>|<span data-ttu-id="bb856-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bb856-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb856-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bb856-128">Request body</span></span>
<span data-ttu-id="bb856-129">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="bb856-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="bb856-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="bb856-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="bb856-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bb856-131">Property</span></span>|<span data-ttu-id="bb856-132">Typ</span><span class="sxs-lookup"><span data-stu-id="bb856-132">Type</span></span>|<span data-ttu-id="bb856-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb856-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb856-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="bb856-134">notificationTitle</span></span>|<span data-ttu-id="bb856-135">String</span><span class="sxs-lookup"><span data-stu-id="bb856-135">String</span></span>|<span data-ttu-id="bb856-136">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="bb856-136">Not yet documented</span></span>|
|<span data-ttu-id="bb856-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="bb856-137">notificationBody</span></span>|<span data-ttu-id="bb856-138">String</span><span class="sxs-lookup"><span data-stu-id="bb856-138">String</span></span>|<span data-ttu-id="bb856-139">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="bb856-139">Not yet documented</span></span>|
|<span data-ttu-id="bb856-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="bb856-140">groupsToNotify</span></span>|<span data-ttu-id="bb856-141">String-Sammlung</span><span class="sxs-lookup"><span data-stu-id="bb856-141">String collection</span></span>|<span data-ttu-id="bb856-142">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="bb856-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="bb856-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb856-143">Response</span></span>
<span data-ttu-id="bb856-144">Wenn die Aktion erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb856-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bb856-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bb856-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb856-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb856-146">Request</span></span>
<span data-ttu-id="bb856-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bb856-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb856-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb856-148">Response</span></span>
<span data-ttu-id="bb856-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb856-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






