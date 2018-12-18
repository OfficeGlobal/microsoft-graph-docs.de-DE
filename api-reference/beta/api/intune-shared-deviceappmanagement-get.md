---
title: Abrufen von „deviceAppManagement“
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs deviceAppManagement.
author: tfitzmac
ms.openlocfilehash: 290a88af983f5c4b4bc6d032b8960c810960d969
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342714"
---
# <a name="get-deviceappmanagement"></a><span data-ttu-id="b4924-103">Abrufen von „deviceAppManagement“</span><span class="sxs-lookup"><span data-stu-id="b4924-103">Get deviceAppManagement</span></span>

> <span data-ttu-id="b4924-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b4924-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4924-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b4924-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4924-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b4924-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4924-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="b4924-107">Read properties and relationships of the [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4924-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b4924-108">Prerequisites</span></span>

<span data-ttu-id="b4924-109">Eine der folgenden Berechtigungen ist erforderlich, um diese API-aufrufen.</span><span class="sxs-lookup"><span data-stu-id="b4924-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b4924-110">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4924-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="b4924-111">Beachten Sie, dass die entsprechende Berechtigungen gemäß den Workflow variiert.</span><span class="sxs-lookup"><span data-stu-id="b4924-111">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="b4924-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4924-112">Permission type</span></span>|<span data-ttu-id="b4924-113">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4924-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="b4924-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4924-114">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="b4924-115">&nbsp;&nbsp; **Apps**, **Bücher**oder **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="b4924-115">&nbsp; &nbsp; **Apps**, **books**, or **onboarding**</span></span> | <span data-ttu-id="b4924-116">DeviceManagementApps.ReadWrite.All DeviceManagementApps.ReadW.All</span><span class="sxs-lookup"><span data-stu-id="b4924-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.ReadW.All</span></span> |
| <span data-ttu-id="b4924-117">&nbsp; &nbsp; **Geräteverwaltung**</span><span class="sxs-lookup"><span data-stu-id="b4924-117">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="b4924-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4924-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
|<span data-ttu-id="b4924-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4924-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4924-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4924-120">Not supported.</span></span>|
|<span data-ttu-id="b4924-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4924-121">Application</span></span>|<span data-ttu-id="b4924-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4924-122">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4924-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4924-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b4924-124">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b4924-124">Optional query parameters</span></span>

<span data-ttu-id="b4924-125">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b4924-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b4924-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4924-126">Request headers</span></span>

|<span data-ttu-id="b4924-127">Header</span><span class="sxs-lookup"><span data-stu-id="b4924-127">Header</span></span>|<span data-ttu-id="b4924-128">Wert</span><span class="sxs-lookup"><span data-stu-id="b4924-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4924-129">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b4924-129">Authorization</span></span>|<span data-ttu-id="b4924-130">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b4924-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4924-131">Accept</span><span class="sxs-lookup"><span data-stu-id="b4924-131">Accept</span></span>|<span data-ttu-id="b4924-132">application/json</span><span class="sxs-lookup"><span data-stu-id="b4924-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4924-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4924-133">Request body</span></span>

<span data-ttu-id="b4924-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b4924-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4924-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4924-135">Response</span></span>

<span data-ttu-id="b4924-136">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b4924-136">If successful, this method returns a `200 OK` response code and [deviceAppManagement](../resources/intune-shared-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4924-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4924-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4924-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4924-138">Request</span></span>

<span data-ttu-id="b4924-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4924-139">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceAppManagement
```

### <a name="response"></a><span data-ttu-id="b4924-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4924-140">Response</span></span>

<span data-ttu-id="b4924-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4924-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



