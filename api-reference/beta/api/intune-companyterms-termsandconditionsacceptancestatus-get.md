---
title: Abrufen von „termsAndConditionsAcceptanceStatus“
description: Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7a759ebdf73a1cbdf9afd1938f4f98c6e5a243b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873976"
---
# <a name="get-termsandconditionsacceptancestatus"></a><span data-ttu-id="d3234-103">Abrufen von „termsAndConditionsAcceptanceStatus“</span><span class="sxs-lookup"><span data-stu-id="d3234-103">Get termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="d3234-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d3234-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3234-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d3234-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d3234-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="d3234-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3234-107">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="d3234-107">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d3234-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d3234-108">Prerequisites</span></span>
<span data-ttu-id="d3234-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3234-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3234-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d3234-111">Permission type</span></span>|<span data-ttu-id="d3234-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d3234-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3234-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d3234-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3234-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3234-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d3234-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d3234-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3234-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3234-116">Not supported.</span></span>|
|<span data-ttu-id="d3234-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d3234-117">Application</span></span>|<span data-ttu-id="d3234-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3234-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3234-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3234-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d3234-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d3234-120">Optional query parameters</span></span>
<span data-ttu-id="d3234-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d3234-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d3234-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d3234-122">Request headers</span></span>
|<span data-ttu-id="d3234-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d3234-123">Header</span></span>|<span data-ttu-id="d3234-124">Wert</span><span class="sxs-lookup"><span data-stu-id="d3234-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3234-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3234-125">Authorization</span></span>|<span data-ttu-id="d3234-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d3234-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3234-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d3234-127">Accept</span></span>|<span data-ttu-id="d3234-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d3234-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3234-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d3234-129">Request body</span></span>
<span data-ttu-id="d3234-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d3234-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3234-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3234-131">Response</span></span>
<span data-ttu-id="d3234-132">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein Objekt des Typs [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d3234-132">If successful, this method returns a `200 OK` response code and [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3234-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d3234-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d3234-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3234-134">Request</span></span>
<span data-ttu-id="d3234-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d3234-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

### <a name="response"></a><span data-ttu-id="d3234-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3234-136">Response</span></span>
<span data-ttu-id="d3234-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d3234-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
    "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
    "userDisplayName": "User Display Name value",
    "acceptedVersion": 15,
    "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
  }
}
```





