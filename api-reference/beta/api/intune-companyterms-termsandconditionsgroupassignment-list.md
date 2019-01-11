---
title: Liste termsAndConditionsGroupAssignments
description: Listeneigenschaften und Beziehungen der TermsAndConditionsGroupAssignment-Objekte.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 14dfed592d46934d0f9b067a56c8e6c74c38924e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832557"
---
# <a name="list-termsandconditionsgroupassignments"></a><span data-ttu-id="6a7c5-103">Liste termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="6a7c5-103">List termsAndConditionsGroupAssignments</span></span>

> <span data-ttu-id="6a7c5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a7c5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a7c5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a7c5-107">Listeneigenschaften und Beziehungen der [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-107">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6a7c5-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6a7c5-108">Prerequisites</span></span>
<span data-ttu-id="6a7c5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a7c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a7c5-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6a7c5-111">Permission type</span></span>|<span data-ttu-id="6a7c5-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6a7c5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a7c5-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6a7c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a7c5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a7c5-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6a7c5-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6a7c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a7c5-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a7c5-116">Not supported.</span></span>|
|<span data-ttu-id="6a7c5-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6a7c5-117">Application</span></span>|<span data-ttu-id="6a7c5-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a7c5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a7c5-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a7c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="6a7c5-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a7c5-120">Request headers</span></span>
|<span data-ttu-id="6a7c5-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6a7c5-121">Header</span></span>|<span data-ttu-id="6a7c5-122">Wert</span><span class="sxs-lookup"><span data-stu-id="6a7c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a7c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a7c5-123">Authorization</span></span>|<span data-ttu-id="6a7c5-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6a7c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a7c5-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6a7c5-125">Accept</span></span>|<span data-ttu-id="6a7c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a7c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a7c5-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a7c5-127">Request body</span></span>
<span data-ttu-id="6a7c5-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a7c5-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a7c5-129">Response</span></span>
<span data-ttu-id="6a7c5-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="6a7c5-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a7c5-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a7c5-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6a7c5-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a7c5-132">Request</span></span>
<span data-ttu-id="6a7c5-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="6a7c5-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a7c5-134">Response</span></span>
<span data-ttu-id="6a7c5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a7c5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 214

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
      "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
      "targetGroupId": "Target Group Id value"
    }
  ]
}
```





