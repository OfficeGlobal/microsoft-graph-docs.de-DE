---
title: telecomExpenseManagementPartner abrufen
description: Lesen von Eigenschaften und Beziehungen des telecomExpenseManagementPartner-Objekts.
author: tfitzmac
ms.openlocfilehash: afca2b07c130167783331c1989911ac065c61268
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354243"
---
# <a name="get-telecomexpensemanagementpartner"></a><span data-ttu-id="386ae-103">telecomExpenseManagementPartner abrufen</span><span class="sxs-lookup"><span data-stu-id="386ae-103">Get telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="386ae-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="386ae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="386ae-105">Lesen von Eigenschaften und Beziehungen des [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="386ae-105">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="386ae-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="386ae-106">Prerequisites</span></span>
<span data-ttu-id="386ae-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="386ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="386ae-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="386ae-109">Permission type</span></span>|<span data-ttu-id="386ae-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="386ae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="386ae-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="386ae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="386ae-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="386ae-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="386ae-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="386ae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="386ae-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="386ae-114">Not supported.</span></span>|
|<span data-ttu-id="386ae-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="386ae-115">Application</span></span>|<span data-ttu-id="386ae-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="386ae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="386ae-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="386ae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="386ae-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="386ae-118">Optional query parameters</span></span>
<span data-ttu-id="386ae-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="386ae-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="386ae-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="386ae-120">Request headers</span></span>
|<span data-ttu-id="386ae-121">Header</span><span class="sxs-lookup"><span data-stu-id="386ae-121">Header</span></span>|<span data-ttu-id="386ae-122">Wert</span><span class="sxs-lookup"><span data-stu-id="386ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="386ae-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="386ae-123">Authorization</span></span>|<span data-ttu-id="386ae-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="386ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="386ae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="386ae-125">Accept</span></span>|<span data-ttu-id="386ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="386ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="386ae-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="386ae-127">Request body</span></span>
<span data-ttu-id="386ae-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="386ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="386ae-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="386ae-129">Response</span></span>
<span data-ttu-id="386ae-130">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="386ae-130">If successful, this method returns a `200 OK` response code and [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="386ae-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="386ae-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="386ae-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="386ae-132">Request</span></span>
<span data-ttu-id="386ae-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="386ae-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="386ae-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="386ae-134">Response</span></span>
<span data-ttu-id="386ae-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="386ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": {
    "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
    "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
    "displayName": "Display Name value",
    "url": "Url value",
    "appAuthorized": true,
    "enabled": true,
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
  }
}
```



