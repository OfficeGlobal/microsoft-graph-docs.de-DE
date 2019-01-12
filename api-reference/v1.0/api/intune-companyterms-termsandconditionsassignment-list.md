---
title: Auflisten von „termsAndConditionsAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs termsAndConditionsAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1c9beea3297c1360ee11a1ed267a5d06e9247862
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962555"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="66890-103">Auflisten von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="66890-103">List termsAndConditionsAssignments</span></span>

> <span data-ttu-id="66890-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="66890-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66890-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="66890-105">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66890-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="66890-106">Prerequisites</span></span>
<span data-ttu-id="66890-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66890-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66890-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66890-109">Permission type</span></span>|<span data-ttu-id="66890-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="66890-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66890-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66890-111">Delegated (work or school account)</span></span>|<span data-ttu-id="66890-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="66890-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="66890-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="66890-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66890-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66890-114">Not supported.</span></span>|
|<span data-ttu-id="66890-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66890-115">Application</span></span>|<span data-ttu-id="66890-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66890-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66890-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66890-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="66890-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66890-118">Request headers</span></span>
|<span data-ttu-id="66890-119">Header</span><span class="sxs-lookup"><span data-stu-id="66890-119">Header</span></span>|<span data-ttu-id="66890-120">Wert</span><span class="sxs-lookup"><span data-stu-id="66890-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66890-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="66890-121">Authorization</span></span>|<span data-ttu-id="66890-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="66890-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66890-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="66890-123">Accept</span></span>|<span data-ttu-id="66890-124">application/json</span><span class="sxs-lookup"><span data-stu-id="66890-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66890-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66890-125">Request body</span></span>
<span data-ttu-id="66890-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="66890-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66890-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="66890-127">Response</span></span>
<span data-ttu-id="66890-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="66890-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66890-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66890-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="66890-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66890-130">Request</span></span>
<span data-ttu-id="66890-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66890-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="66890-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="66890-132">Response</span></span>
<span data-ttu-id="66890-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66890-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



