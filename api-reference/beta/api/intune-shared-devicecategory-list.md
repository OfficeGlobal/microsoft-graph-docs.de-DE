---
title: Auflisten von „deviceCategory“
description: Auflisten von Eigenschaften und Beziehungen der deviceCategory-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 857d9db112853fe85c51df342e66b6bcaff7cfd0
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572502"
---
# <a name="list-devicecategories"></a><span data-ttu-id="7b0ed-103">Auflisten von „deviceCategory“</span><span class="sxs-lookup"><span data-stu-id="7b0ed-103">List deviceCategories</span></span>

> <span data-ttu-id="7b0ed-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="7b0ed-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7b0ed-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7b0ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b0ed-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7b0ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b0ed-107">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) auf.</span><span class="sxs-lookup"><span data-stu-id="7b0ed-107">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7b0ed-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7b0ed-108">Prerequisites</span></span>
<span data-ttu-id="7b0ed-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b0ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7b0ed-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b0ed-111">Permission type</span></span>|<span data-ttu-id="7b0ed-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b0ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b0ed-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b0ed-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7b0ed-114">&nbsp; &nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="7b0ed-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7b0ed-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b0ed-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="7b0ed-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b0ed-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b0ed-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b0ed-117">Not supported.</span></span>|
|<span data-ttu-id="7b0ed-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b0ed-118">Application</span></span>|<span data-ttu-id="7b0ed-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b0ed-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b0ed-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b0ed-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="7b0ed-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b0ed-121">Request headers</span></span>

|<span data-ttu-id="7b0ed-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7b0ed-122">Header</span></span>|<span data-ttu-id="7b0ed-123">Wert</span><span class="sxs-lookup"><span data-stu-id="7b0ed-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b0ed-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b0ed-124">Authorization</span></span>|<span data-ttu-id="7b0ed-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="7b0ed-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b0ed-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="7b0ed-126">Accept</span></span>|<span data-ttu-id="7b0ed-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7b0ed-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b0ed-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b0ed-128">Request body</span></span>

<span data-ttu-id="7b0ed-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7b0ed-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b0ed-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b0ed-130">Response</span></span>

<span data-ttu-id="7b0ed-131">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [deviceCategory](../resources/intune-shared-devicecategory.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7b0ed-131">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b0ed-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b0ed-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b0ed-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b0ed-133">Request</span></span>

<span data-ttu-id="7b0ed-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b0ed-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="7b0ed-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b0ed-135">Response</span></span>

<span data-ttu-id="7b0ed-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b0ed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



