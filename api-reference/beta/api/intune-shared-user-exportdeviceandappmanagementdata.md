---
title: ExportDeviceAndAppManagementData-Funktion
description: Noch nicht dokumentiert
ms.openlocfilehash: fdcf75817d3fae157480b4e232bf4052ac84f64b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059143"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="4a3db-103">ExportDeviceAndAppManagementData-Funktion</span><span class="sxs-lookup"><span data-stu-id="4a3db-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="4a3db-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4a3db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a3db-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4a3db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a3db-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4a3db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a3db-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4a3db-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a3db-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4a3db-108">Prerequisites</span></span>

<span data-ttu-id="4a3db-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a3db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a3db-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a3db-111">Permission type</span></span>|<span data-ttu-id="4a3db-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a3db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a3db-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a3db-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4a3db-114">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="4a3db-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="4a3db-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a3db-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4a3db-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a3db-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a3db-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a3db-117">Not supported.</span></span>|
|<span data-ttu-id="4a3db-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a3db-118">Application</span></span>|<span data-ttu-id="4a3db-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a3db-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a3db-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a3db-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="4a3db-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a3db-121">Request headers</span></span>

|<span data-ttu-id="4a3db-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4a3db-122">Header</span></span>|<span data-ttu-id="4a3db-123">Wert</span><span class="sxs-lookup"><span data-stu-id="4a3db-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a3db-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a3db-124">Authorization</span></span>|<span data-ttu-id="4a3db-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4a3db-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a3db-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4a3db-126">Accept</span></span>|<span data-ttu-id="4a3db-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4a3db-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a3db-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a3db-128">Request body</span></span>

<span data-ttu-id="4a3db-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="4a3db-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4a3db-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4a3db-130">Property</span></span>|<span data-ttu-id="4a3db-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4a3db-131">Type</span></span>|<span data-ttu-id="4a3db-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a3db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a3db-133">skip</span><span class="sxs-lookup"><span data-stu-id="4a3db-133">skip</span></span>|<span data-ttu-id="4a3db-134">Int32</span><span class="sxs-lookup"><span data-stu-id="4a3db-134">Int32</span></span>|<span data-ttu-id="4a3db-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4a3db-135">Not yet documented</span></span>|
|<span data-ttu-id="4a3db-136">Nach oben</span><span class="sxs-lookup"><span data-stu-id="4a3db-136">top</span></span>|<span data-ttu-id="4a3db-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4a3db-137">Int32</span></span>|<span data-ttu-id="4a3db-138">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4a3db-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="4a3db-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a3db-139">Response</span></span>

<span data-ttu-id="4a3db-140">Wenn erfolgreich, diese Funktion gibt eine `200 OK` Antwortcode und eine [DeviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4a3db-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a3db-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a3db-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a3db-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a3db-142">Request</span></span>

<span data-ttu-id="4a3db-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4a3db-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="4a3db-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a3db-144">Response</span></span>

<span data-ttu-id="4a3db-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a3db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



