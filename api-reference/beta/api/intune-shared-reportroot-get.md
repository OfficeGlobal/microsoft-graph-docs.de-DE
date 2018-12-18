---
title: Abrufen von „reportRoot“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs reportRoot.
author: tfitzmac
ms.openlocfilehash: 9c33b39dd3bf504c1ebfaad7ca41ca19eff69975
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316324"
---
# <a name="get-reportroot"></a><span data-ttu-id="da2b4-103">Abrufen von „reportRoot“</span><span class="sxs-lookup"><span data-stu-id="da2b4-103">Get reportRoot</span></span>

> <span data-ttu-id="da2b4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="da2b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da2b4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da2b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da2b4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="da2b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da2b4-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="da2b4-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da2b4-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="da2b4-108">Prerequisites</span></span>
<span data-ttu-id="da2b4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da2b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da2b4-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="da2b4-111">Permission type</span></span>|<span data-ttu-id="da2b4-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="da2b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da2b4-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="da2b4-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="da2b4-114">&nbsp;&nbsp; **Gerätekonfiguration**</span><span class="sxs-lookup"><span data-stu-id="da2b4-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="da2b4-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="da2b4-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="da2b4-116">&nbsp; &nbsp; **Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="da2b4-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="da2b4-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="da2b4-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="da2b4-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="da2b4-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da2b4-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da2b4-119">Not supported.</span></span>|
|<span data-ttu-id="da2b4-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="da2b4-120">Application</span></span>|<span data-ttu-id="da2b4-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="da2b4-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da2b4-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="da2b4-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da2b4-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="da2b4-123">Optional query parameters</span></span>
<span data-ttu-id="da2b4-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="da2b4-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="da2b4-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="da2b4-125">Request headers</span></span>
|<span data-ttu-id="da2b4-126">Header</span><span class="sxs-lookup"><span data-stu-id="da2b4-126">Header</span></span>|<span data-ttu-id="da2b4-127">Wert</span><span class="sxs-lookup"><span data-stu-id="da2b4-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da2b4-128">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="da2b4-128">Authorization</span></span>|<span data-ttu-id="da2b4-129">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="da2b4-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da2b4-130">Accept</span><span class="sxs-lookup"><span data-stu-id="da2b4-130">Accept</span></span>|<span data-ttu-id="da2b4-131">application/json</span><span class="sxs-lookup"><span data-stu-id="da2b4-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da2b4-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="da2b4-132">Request body</span></span>
<span data-ttu-id="da2b4-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="da2b4-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da2b4-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="da2b4-134">Response</span></span>
<span data-ttu-id="da2b4-135">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [reportRoot](../resources/intune-shared-reportroot.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="da2b4-135">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da2b4-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="da2b4-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="da2b4-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="da2b4-137">Request</span></span>
<span data-ttu-id="da2b4-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="da2b4-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="da2b4-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="da2b4-139">Response</span></span>
<span data-ttu-id="da2b4-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="da2b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```



