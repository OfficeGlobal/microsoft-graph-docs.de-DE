---
title: ExportDeviceAndAppManagementData-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c7c4bc294d382cf1e1917a2c5a607a7c90107856
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872846"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="df0bc-103">ExportDeviceAndAppManagementData-Funktion</span><span class="sxs-lookup"><span data-stu-id="df0bc-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="df0bc-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df0bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df0bc-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df0bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df0bc-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="df0bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df0bc-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="df0bc-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df0bc-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="df0bc-108">Prerequisites</span></span>

<span data-ttu-id="df0bc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df0bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df0bc-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="df0bc-111">Permission type</span></span>|<span data-ttu-id="df0bc-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="df0bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df0bc-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="df0bc-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="df0bc-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="df0bc-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="df0bc-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df0bc-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df0bc-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="df0bc-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df0bc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df0bc-117">Not supported.</span></span>|
|<span data-ttu-id="df0bc-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="df0bc-118">Application</span></span>|<span data-ttu-id="df0bc-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="df0bc-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df0bc-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="df0bc-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="df0bc-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="df0bc-121">Request headers</span></span>

|<span data-ttu-id="df0bc-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="df0bc-122">Header</span></span>|<span data-ttu-id="df0bc-123">Wert</span><span class="sxs-lookup"><span data-stu-id="df0bc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df0bc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="df0bc-124">Authorization</span></span>|<span data-ttu-id="df0bc-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="df0bc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df0bc-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="df0bc-126">Accept</span></span>|<span data-ttu-id="df0bc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="df0bc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df0bc-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="df0bc-128">Request body</span></span>

<span data-ttu-id="df0bc-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="df0bc-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="df0bc-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df0bc-130">Property</span></span>|<span data-ttu-id="df0bc-131">Typ</span><span class="sxs-lookup"><span data-stu-id="df0bc-131">Type</span></span>|<span data-ttu-id="df0bc-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df0bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df0bc-133">skip</span><span class="sxs-lookup"><span data-stu-id="df0bc-133">skip</span></span>|<span data-ttu-id="df0bc-134">Int32</span><span class="sxs-lookup"><span data-stu-id="df0bc-134">Int32</span></span>|<span data-ttu-id="df0bc-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="df0bc-135">Not yet documented</span></span>|
|<span data-ttu-id="df0bc-136">Nach oben</span><span class="sxs-lookup"><span data-stu-id="df0bc-136">top</span></span>|<span data-ttu-id="df0bc-137">Int32</span><span class="sxs-lookup"><span data-stu-id="df0bc-137">Int32</span></span>|<span data-ttu-id="df0bc-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="df0bc-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="df0bc-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="df0bc-139">Response</span></span>

<span data-ttu-id="df0bc-140">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [DeviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="df0bc-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df0bc-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="df0bc-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="df0bc-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="df0bc-142">Request</span></span>

<span data-ttu-id="df0bc-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="df0bc-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="df0bc-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="df0bc-144">Response</span></span>

<span data-ttu-id="df0bc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="df0bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementData",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```



