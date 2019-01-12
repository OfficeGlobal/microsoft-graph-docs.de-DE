---
title: ExportDeviceAndAppManagementData-Funktion
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5ab337ccca261dde98d609434fa7948bc07bcfca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965110"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="d5495-103">ExportDeviceAndAppManagementData-Funktion</span><span class="sxs-lookup"><span data-stu-id="d5495-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="d5495-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d5495-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5495-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d5495-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5495-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d5495-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5495-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d5495-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5495-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d5495-108">Prerequisites</span></span>

<span data-ttu-id="d5495-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5495-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5495-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d5495-111">Permission type</span></span>|<span data-ttu-id="d5495-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d5495-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5495-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d5495-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="d5495-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="d5495-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="d5495-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5495-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d5495-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d5495-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5495-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5495-117">Not supported.</span></span>|
|<span data-ttu-id="d5495-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d5495-118">Application</span></span>|<span data-ttu-id="d5495-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d5495-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5495-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5495-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="d5495-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d5495-121">Request headers</span></span>

|<span data-ttu-id="d5495-122">Header</span><span class="sxs-lookup"><span data-stu-id="d5495-122">Header</span></span>|<span data-ttu-id="d5495-123">Wert</span><span class="sxs-lookup"><span data-stu-id="d5495-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5495-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5495-124">Authorization</span></span>|<span data-ttu-id="d5495-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d5495-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5495-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d5495-126">Accept</span></span>|<span data-ttu-id="d5495-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d5495-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5495-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d5495-128">Request body</span></span>

<span data-ttu-id="d5495-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="d5495-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d5495-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d5495-130">Property</span></span>|<span data-ttu-id="d5495-131">Typ</span><span class="sxs-lookup"><span data-stu-id="d5495-131">Type</span></span>|<span data-ttu-id="d5495-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d5495-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5495-133">skip</span><span class="sxs-lookup"><span data-stu-id="d5495-133">skip</span></span>|<span data-ttu-id="d5495-134">Int32</span><span class="sxs-lookup"><span data-stu-id="d5495-134">Int32</span></span>|<span data-ttu-id="d5495-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d5495-135">Not yet documented</span></span>|
|<span data-ttu-id="d5495-136">Nach oben</span><span class="sxs-lookup"><span data-stu-id="d5495-136">top</span></span>|<span data-ttu-id="d5495-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d5495-137">Int32</span></span>|<span data-ttu-id="d5495-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d5495-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="d5495-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5495-139">Response</span></span>

<span data-ttu-id="d5495-140">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [DeviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="d5495-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5495-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d5495-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5495-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d5495-142">Request</span></span>

<span data-ttu-id="d5495-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d5495-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="d5495-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="d5495-144">Response</span></span>

<span data-ttu-id="d5495-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d5495-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



