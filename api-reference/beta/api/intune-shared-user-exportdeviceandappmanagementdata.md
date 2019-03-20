---
title: exportDeviceAndAppManagementData-Funktion
description: Noch nicht dokumentiert.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a2e776d885a2f4374251fbb57b10377c03fbb8ec
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572299"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="ed077-103">exportDeviceAndAppManagementData-Funktion</span><span class="sxs-lookup"><span data-stu-id="ed077-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="ed077-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="ed077-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ed077-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed077-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed077-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ed077-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed077-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="ed077-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed077-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ed077-108">Prerequisites</span></span>

<span data-ttu-id="ed077-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ed077-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ed077-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed077-111">Permission type</span></span>|<span data-ttu-id="ed077-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed077-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed077-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed077-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ed077-114">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="ed077-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ed077-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed077-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ed077-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed077-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed077-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed077-117">Not supported.</span></span>|
|<span data-ttu-id="ed077-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed077-118">Application</span></span>|<span data-ttu-id="ed077-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed077-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed077-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed077-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="ed077-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed077-121">Request headers</span></span>

|<span data-ttu-id="ed077-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ed077-122">Header</span></span>|<span data-ttu-id="ed077-123">Wert</span><span class="sxs-lookup"><span data-stu-id="ed077-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed077-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed077-124">Authorization</span></span>|<span data-ttu-id="ed077-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ed077-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed077-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ed077-126">Accept</span></span>|<span data-ttu-id="ed077-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ed077-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed077-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed077-128">Request body</span></span>

<span data-ttu-id="ed077-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Funktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="ed077-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ed077-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed077-130">Property</span></span>|<span data-ttu-id="ed077-131">Typ</span><span class="sxs-lookup"><span data-stu-id="ed077-131">Type</span></span>|<span data-ttu-id="ed077-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed077-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed077-133">skip</span><span class="sxs-lookup"><span data-stu-id="ed077-133">skip</span></span>|<span data-ttu-id="ed077-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ed077-134">Int32</span></span>|<span data-ttu-id="ed077-135">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ed077-135">Not yet documented</span></span>|
|<span data-ttu-id="ed077-136">top</span><span class="sxs-lookup"><span data-stu-id="ed077-136">top</span></span>|<span data-ttu-id="ed077-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ed077-137">Int32</span></span>|<span data-ttu-id="ed077-138">Noch nicht dokumentiert.</span><span class="sxs-lookup"><span data-stu-id="ed077-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="ed077-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed077-139">Response</span></span>

<span data-ttu-id="ed077-140">Bei erfolgreicher Ausführung gibt die Funktion den `200 OK` Antwortcode und eine [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ed077-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed077-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed077-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed077-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed077-142">Request</span></span>

<span data-ttu-id="ed077-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed077-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="ed077-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed077-144">Response</span></span>

<span data-ttu-id="ed077-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed077-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



