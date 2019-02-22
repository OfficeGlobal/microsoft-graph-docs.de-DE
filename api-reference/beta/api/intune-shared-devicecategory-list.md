---
title: Auflisten von „deviceCategory“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceCategory auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 40f138305b9f148bb48c4d4398024a8766a2bd5f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169321"
---
# <a name="list-devicecategories"></a><span data-ttu-id="bd764-103">Auflisten von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="bd764-103">List deviceCategories</span></span>

> <span data-ttu-id="bd764-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="bd764-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd764-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd764-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd764-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bd764-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd764-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) auf.</span><span class="sxs-lookup"><span data-stu-id="bd764-107">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd764-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bd764-108">Prerequisites</span></span>
<span data-ttu-id="bd764-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd764-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="bd764-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd764-111">Permission type</span></span>|<span data-ttu-id="bd764-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd764-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd764-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd764-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="bd764-114">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="bd764-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="bd764-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd764-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="bd764-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd764-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd764-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd764-117">Not supported.</span></span>|
|<span data-ttu-id="bd764-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd764-118">Application</span></span>|<span data-ttu-id="bd764-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd764-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd764-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd764-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="bd764-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd764-121">Request headers</span></span>

|<span data-ttu-id="bd764-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bd764-122">Header</span></span>|<span data-ttu-id="bd764-123">Wert</span><span class="sxs-lookup"><span data-stu-id="bd764-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd764-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd764-124">Authorization</span></span>|<span data-ttu-id="bd764-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bd764-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd764-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bd764-126">Accept</span></span>|<span data-ttu-id="bd764-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bd764-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd764-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd764-128">Request body</span></span>

<span data-ttu-id="bd764-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bd764-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd764-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd764-130">Response</span></span>

<span data-ttu-id="bd764-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bd764-131">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd764-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bd764-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd764-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd764-133">Request</span></span>

<span data-ttu-id="bd764-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bd764-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="bd764-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd764-135">Response</span></span>

<span data-ttu-id="bd764-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd764-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCategory",
      "id": "f881b841-b841-f881-41b8-81f841b881f8",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```



