---
title: Abrufen von „deviceAppManagement“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs deviceAppManagement.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7a7bc478dc4a9a59b067b5acb3688c0bb0793d9f
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570822"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="1f05e-103">Abrufen von „deviceAppManagement“</span><span class="sxs-lookup"><span data-stu-id="1f05e-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="1f05e-104">**Wichtig:** APIs unter der/Beta-Version in Microsoft Graph können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="1f05e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1f05e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1f05e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f05e-106">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1f05e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f05e-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="1f05e-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f05e-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1f05e-108">Prerequisites</span></span>

<span data-ttu-id="1f05e-109">Eine der folgenden Berechtigungen ist erforderlich, um diese API aufzurufen.</span><span class="sxs-lookup"><span data-stu-id="1f05e-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="1f05e-110">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1f05e-110">To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>  <span data-ttu-id="1f05e-111">Beachten Sie, dass die entsprechende Berechtigung je nach Workflow variiert.</span><span class="sxs-lookup"><span data-stu-id="1f05e-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="1f05e-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1f05e-112">Permission type</span></span>|<span data-ttu-id="1f05e-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1f05e-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="1f05e-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1f05e-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="1f05e-115">&nbsp;&nbsp; **Apps**, **Bücher**oder Onboarding \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="1f05e-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="1f05e-116">DeviceManagementApps. ReadWrite. all, DeviceManagementApps. ReadW. all</span><span class="sxs-lookup"><span data-stu-id="1f05e-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="1f05e-117">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="1f05e-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="1f05e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f05e-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="1f05e-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1f05e-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f05e-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f05e-120">Not supported.</span></span>|
|<span data-ttu-id="1f05e-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1f05e-121">Application</span></span>|<span data-ttu-id="1f05e-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1f05e-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f05e-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f05e-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1f05e-124">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1f05e-124">Optional query parameters</span></span>

<span data-ttu-id="1f05e-125">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1f05e-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1f05e-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1f05e-126">Request headers</span></span>

|<span data-ttu-id="1f05e-127">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1f05e-127">Header</span></span>|<span data-ttu-id="1f05e-128">Wert</span><span class="sxs-lookup"><span data-stu-id="1f05e-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f05e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f05e-129">Authorization</span></span>|<span data-ttu-id="1f05e-130">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1f05e-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f05e-131">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1f05e-131">Accept</span></span>|<span data-ttu-id="1f05e-132">application/json</span><span class="sxs-lookup"><span data-stu-id="1f05e-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f05e-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1f05e-133">Request body</span></span>

<span data-ttu-id="1f05e-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1f05e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f05e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f05e-135">Response</span></span>

<span data-ttu-id="1f05e-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1f05e-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f05e-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1f05e-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f05e-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1f05e-138">Request</span></span>

<span data-ttu-id="1f05e-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1f05e-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="1f05e-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1f05e-140">Response</span></span>

<span data-ttu-id="1f05e-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1f05e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 133

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAppManagement",
    "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
  }
}
```



