---
title: termsAndConditions abrufen
description: Liest die Eigenschaften und Beziehungen von Objekten des Typs termsAndConditions.
author: tfitzmac
ms.openlocfilehash: 36b3bae881558a0f0122cc887cd6e5373a988894
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354278"
---
# <a name="get-termsandconditions"></a><span data-ttu-id="869c7-103">termsAndConditions abrufen</span><span class="sxs-lookup"><span data-stu-id="869c7-103">Get termsAndConditions</span></span>

> <span data-ttu-id="869c7-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="869c7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="869c7-105">Liest die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="869c7-105">Read properties and relationships of the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="869c7-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="869c7-106">Prerequisites</span></span>
<span data-ttu-id="869c7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="869c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="869c7-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="869c7-109">Permission type</span></span>|<span data-ttu-id="869c7-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="869c7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="869c7-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="869c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="869c7-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="869c7-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="869c7-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="869c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="869c7-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="869c7-114">Not supported.</span></span>|
|<span data-ttu-id="869c7-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="869c7-115">Application</span></span>|<span data-ttu-id="869c7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="869c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="869c7-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="869c7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="869c7-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="869c7-118">Optional query parameters</span></span>
<span data-ttu-id="869c7-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="869c7-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="869c7-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="869c7-120">Request headers</span></span>
|<span data-ttu-id="869c7-121">Header</span><span class="sxs-lookup"><span data-stu-id="869c7-121">Header</span></span>|<span data-ttu-id="869c7-122">Wert</span><span class="sxs-lookup"><span data-stu-id="869c7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="869c7-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="869c7-123">Authorization</span></span>|<span data-ttu-id="869c7-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="869c7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="869c7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="869c7-125">Accept</span></span>|<span data-ttu-id="869c7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="869c7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="869c7-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="869c7-127">Request body</span></span>
<span data-ttu-id="869c7-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="869c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="869c7-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="869c7-129">Response</span></span>
<span data-ttu-id="869c7-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="869c7-130">If successful, this method returns a `200 OK` response code and [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="869c7-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="869c7-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="869c7-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="869c7-132">Request</span></span>
<span data-ttu-id="869c7-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="869c7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
```

### <a name="response"></a><span data-ttu-id="869c7-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="869c7-134">Response</span></span>
<span data-ttu-id="869c7-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="869c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditions",
    "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "title": "Title value",
    "bodyText": "Body Text value",
    "acceptanceStatement": "Acceptance Statement value",
    "version": 7
  }
}
```



