---
title: Auflisten von „deviceCategory“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs deviceCategory auf.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a639bb8f3c5d9c796a0d62e6e32fbd53526a7a0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890888"
---
# <a name="list-devicecategories"></a><span data-ttu-id="57f18-103">Auflisten von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="57f18-103">List deviceCategories</span></span>

> <span data-ttu-id="57f18-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="57f18-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57f18-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) auf.</span><span class="sxs-lookup"><span data-stu-id="57f18-105">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57f18-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="57f18-106">Prerequisites</span></span>
<span data-ttu-id="57f18-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57f18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57f18-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="57f18-109">Permission type</span></span>|<span data-ttu-id="57f18-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="57f18-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57f18-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="57f18-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="57f18-112">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="57f18-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="57f18-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="57f18-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="57f18-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="57f18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57f18-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57f18-115">Not supported.</span></span>|
|<span data-ttu-id="57f18-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="57f18-116">Application</span></span>|<span data-ttu-id="57f18-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="57f18-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57f18-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="57f18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="57f18-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="57f18-119">Request headers</span></span>
|<span data-ttu-id="57f18-120">Header</span><span class="sxs-lookup"><span data-stu-id="57f18-120">Header</span></span>|<span data-ttu-id="57f18-121">Wert</span><span class="sxs-lookup"><span data-stu-id="57f18-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57f18-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="57f18-122">Authorization</span></span>|<span data-ttu-id="57f18-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="57f18-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57f18-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="57f18-124">Accept</span></span>|<span data-ttu-id="57f18-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57f18-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57f18-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="57f18-126">Request body</span></span>
<span data-ttu-id="57f18-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="57f18-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57f18-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="57f18-128">Response</span></span>
<span data-ttu-id="57f18-129">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="57f18-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57f18-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="57f18-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="57f18-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="57f18-131">Request</span></span>
<span data-ttu-id="57f18-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="57f18-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="57f18-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="57f18-133">Response</span></span>
<span data-ttu-id="57f18-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="57f18-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



