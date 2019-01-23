---
title: SendCustomNotificationToCompanyPortal Aktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43e0a5a9690d3f60f646eb5ed55e6d51ba2caab8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418666"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="eb9ac-103">SendCustomNotificationToCompanyPortal Aktion</span><span class="sxs-lookup"><span data-stu-id="eb9ac-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="eb9ac-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="eb9ac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eb9ac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eb9ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb9ac-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eb9ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb9ac-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="eb9ac-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eb9ac-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="eb9ac-108">Prerequisites</span></span>
<span data-ttu-id="eb9ac-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb9ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb9ac-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eb9ac-111">Permission type</span></span>|<span data-ttu-id="eb9ac-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eb9ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb9ac-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eb9ac-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="eb9ac-114">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="eb9ac-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="eb9ac-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb9ac-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="eb9ac-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eb9ac-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb9ac-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb9ac-117">Not supported.</span></span>|
|<span data-ttu-id="eb9ac-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eb9ac-118">Application</span></span>|<span data-ttu-id="eb9ac-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eb9ac-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb9ac-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb9ac-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="eb9ac-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eb9ac-121">Request headers</span></span>
|<span data-ttu-id="eb9ac-122">Header</span><span class="sxs-lookup"><span data-stu-id="eb9ac-122">Header</span></span>|<span data-ttu-id="eb9ac-123">Wert</span><span class="sxs-lookup"><span data-stu-id="eb9ac-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb9ac-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="eb9ac-124">Authorization</span></span>|<span data-ttu-id="eb9ac-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="eb9ac-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb9ac-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="eb9ac-126">Accept</span></span>|<span data-ttu-id="eb9ac-127">application/json</span><span class="sxs-lookup"><span data-stu-id="eb9ac-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb9ac-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eb9ac-128">Request body</span></span>
<span data-ttu-id="eb9ac-129">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="eb9ac-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="eb9ac-130">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="eb9ac-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="eb9ac-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="eb9ac-131">Property</span></span>|<span data-ttu-id="eb9ac-132">Typ</span><span class="sxs-lookup"><span data-stu-id="eb9ac-132">Type</span></span>|<span data-ttu-id="eb9ac-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eb9ac-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb9ac-134">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="eb9ac-134">notificationTitle</span></span>|<span data-ttu-id="eb9ac-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb9ac-135">String</span></span>|<span data-ttu-id="eb9ac-136">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="eb9ac-136">Not yet documented</span></span>|
|<span data-ttu-id="eb9ac-137">notificationBody</span><span class="sxs-lookup"><span data-stu-id="eb9ac-137">notificationBody</span></span>|<span data-ttu-id="eb9ac-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="eb9ac-138">String</span></span>|<span data-ttu-id="eb9ac-139">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="eb9ac-139">Not yet documented</span></span>|
|<span data-ttu-id="eb9ac-140">groupsToNotify</span><span class="sxs-lookup"><span data-stu-id="eb9ac-140">groupsToNotify</span></span>|<span data-ttu-id="eb9ac-141">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="eb9ac-141">String collection</span></span>|<span data-ttu-id="eb9ac-142">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="eb9ac-142">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="eb9ac-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb9ac-143">Response</span></span>
<span data-ttu-id="eb9ac-144">Bei erfolgreicher Ausführung gibt die Aktion den Antwortcode `204 No Content` zurück.</span><span class="sxs-lookup"><span data-stu-id="eb9ac-144">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eb9ac-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eb9ac-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="eb9ac-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eb9ac-146">Request</span></span>
<span data-ttu-id="eb9ac-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eb9ac-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eb9ac-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="eb9ac-148">Response</span></span>
<span data-ttu-id="eb9ac-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eb9ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






