---
title: Auflisten von „termsAndConditionsAssignment“
description: Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs termsAndConditionsAssignment auf.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c2ea2ab60c731e68b862b7bebb46ec966d374fe
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251153"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="533f6-103">Auflisten von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="533f6-103">List termsAndConditionsAssignments</span></span>

> <span data-ttu-id="533f6-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="533f6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="533f6-105">Diese Methode listet die Eigenschaften und Beziehungen von Objekten des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) auf.</span><span class="sxs-lookup"><span data-stu-id="533f6-105">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="533f6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="533f6-106">Prerequisites</span></span>
<span data-ttu-id="533f6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="533f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="533f6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="533f6-109">Permission type</span></span>|<span data-ttu-id="533f6-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="533f6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="533f6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="533f6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="533f6-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="533f6-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="533f6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="533f6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="533f6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="533f6-114">Not supported.</span></span>|
|<span data-ttu-id="533f6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="533f6-115">Application</span></span>|<span data-ttu-id="533f6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="533f6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="533f6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="533f6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="533f6-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="533f6-118">Request headers</span></span>
|<span data-ttu-id="533f6-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="533f6-119">Header</span></span>|<span data-ttu-id="533f6-120">Wert</span><span class="sxs-lookup"><span data-stu-id="533f6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="533f6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="533f6-121">Authorization</span></span>|<span data-ttu-id="533f6-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="533f6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="533f6-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="533f6-123">Accept</span></span>|<span data-ttu-id="533f6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="533f6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="533f6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="533f6-125">Request body</span></span>
<span data-ttu-id="533f6-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="533f6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="533f6-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="533f6-127">Response</span></span>
<span data-ttu-id="533f6-128">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und eine Collection von Objekten des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="533f6-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="533f6-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="533f6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="533f6-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="533f6-130">Request</span></span>
<span data-ttu-id="533f6-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="533f6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="533f6-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="533f6-132">Response</span></span>
<span data-ttu-id="533f6-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="533f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



