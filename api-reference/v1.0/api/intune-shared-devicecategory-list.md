---
title: Auflisten von „deviceCategory“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceCategory auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ed9a6facc72bc941b3e26a802d324e1354d339a6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252084"
---
# <a name="list-devicecategories"></a><span data-ttu-id="9349f-103">Auflisten von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="9349f-103">List deviceCategories</span></span>

> <span data-ttu-id="9349f-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9349f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9349f-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) auf.</span><span class="sxs-lookup"><span data-stu-id="9349f-105">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9349f-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9349f-106">Prerequisites</span></span>
<span data-ttu-id="9349f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9349f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9349f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9349f-109">Permission type</span></span>|<span data-ttu-id="9349f-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9349f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9349f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9349f-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9349f-112">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="9349f-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="9349f-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9349f-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9349f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9349f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9349f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9349f-115">Not supported.</span></span>|
|<span data-ttu-id="9349f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9349f-116">Application</span></span>|<span data-ttu-id="9349f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9349f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9349f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9349f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="9349f-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9349f-119">Request headers</span></span>
|<span data-ttu-id="9349f-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9349f-120">Header</span></span>|<span data-ttu-id="9349f-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9349f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9349f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9349f-122">Authorization</span></span>|<span data-ttu-id="9349f-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9349f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9349f-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9349f-124">Accept</span></span>|<span data-ttu-id="9349f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9349f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9349f-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9349f-126">Request body</span></span>
<span data-ttu-id="9349f-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9349f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9349f-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="9349f-128">Response</span></span>
<span data-ttu-id="9349f-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9349f-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9349f-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9349f-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="9349f-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9349f-131">Request</span></span>
<span data-ttu-id="9349f-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9349f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="9349f-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9349f-133">Response</span></span>
<span data-ttu-id="9349f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9349f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



