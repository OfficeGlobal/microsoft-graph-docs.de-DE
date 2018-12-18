---
title: Abrufen von termsAndConditionsGroupAssignment
description: Lesen Sie Eigenschaften und Beziehungen des TermsAndConditionsGroupAssignment-Objekts.
author: tfitzmac
ms.openlocfilehash: 92b9f6c0d48fe09149efd98015d64e96e2575852
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345031"
---
# <a name="get-termsandconditionsgroupassignment"></a><span data-ttu-id="cf610-103">Abrufen von termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="cf610-103">Get termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="cf610-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cf610-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf610-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cf610-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf610-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cf610-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf610-107">Lesen Sie Eigenschaften und Beziehungen des [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cf610-107">Read properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf610-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cf610-108">Prerequisites</span></span>
<span data-ttu-id="cf610-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf610-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf610-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf610-111">Permission type</span></span>|<span data-ttu-id="cf610-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf610-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf610-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf610-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf610-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf610-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="cf610-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf610-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf610-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf610-116">Not supported.</span></span>|
|<span data-ttu-id="cf610-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf610-117">Application</span></span>|<span data-ttu-id="cf610-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf610-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf610-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf610-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf610-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cf610-120">Optional query parameters</span></span>
<span data-ttu-id="cf610-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cf610-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cf610-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf610-122">Request headers</span></span>
|<span data-ttu-id="cf610-123">Header</span><span class="sxs-lookup"><span data-stu-id="cf610-123">Header</span></span>|<span data-ttu-id="cf610-124">Wert</span><span class="sxs-lookup"><span data-stu-id="cf610-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf610-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="cf610-125">Authorization</span></span>|<span data-ttu-id="cf610-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cf610-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf610-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cf610-127">Accept</span></span>|<span data-ttu-id="cf610-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cf610-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf610-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf610-129">Request body</span></span>
<span data-ttu-id="cf610-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cf610-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf610-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf610-131">Response</span></span>
<span data-ttu-id="cf610-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="cf610-132">If successful, this method returns a `200 OK` response code and [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf610-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf610-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf610-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf610-134">Request</span></span>
<span data-ttu-id="cf610-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf610-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="cf610-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf610-136">Response</span></span>
<span data-ttu-id="cf610-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf610-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 194

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
    "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
    "targetGroupId": "Target Group Id value"
  }
}
```





