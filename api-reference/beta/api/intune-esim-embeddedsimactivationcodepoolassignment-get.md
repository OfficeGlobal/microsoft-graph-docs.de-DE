---
title: Abrufen von embeddedSIMActivationCodePoolAssignment
description: Lesen Sie Eigenschaften und Beziehungen des EmbeddedSIMActivationCodePoolAssignment-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6b902a2cbb6a4b2aaef786a6bf5a8086ea251d92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394551"
---
# <a name="get-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="5b6a8-103">Abrufen von embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="5b6a8-103">Get embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="5b6a8-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5b6a8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b6a8-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b6a8-107">Lesen Sie Eigenschaften und Beziehungen des [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-107">Read properties and relationships of the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b6a8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="5b6a8-108">Prerequisites</span></span>
<span data-ttu-id="5b6a8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5b6a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5b6a8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b6a8-111">Permission type</span></span>|<span data-ttu-id="5b6a8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b6a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b6a8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b6a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b6a8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b6a8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5b6a8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b6a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b6a8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b6a8-116">Not supported.</span></span>|
|<span data-ttu-id="5b6a8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b6a8-117">Application</span></span>|<span data-ttu-id="5b6a8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b6a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b6a8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b6a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b6a8-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5b6a8-120">Optional query parameters</span></span>
<span data-ttu-id="5b6a8-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5b6a8-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b6a8-122">Request headers</span></span>
|<span data-ttu-id="5b6a8-123">Header</span><span class="sxs-lookup"><span data-stu-id="5b6a8-123">Header</span></span>|<span data-ttu-id="5b6a8-124">Wert</span><span class="sxs-lookup"><span data-stu-id="5b6a8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b6a8-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="5b6a8-125">Authorization</span></span>|<span data-ttu-id="5b6a8-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="5b6a8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b6a8-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5b6a8-127">Accept</span></span>|<span data-ttu-id="5b6a8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5b6a8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b6a8-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b6a8-129">Request body</span></span>
<span data-ttu-id="5b6a8-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b6a8-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b6a8-131">Response</span></span>
<span data-ttu-id="5b6a8-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-132">If successful, this method returns a `200 OK` response code and [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b6a8-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b6a8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b6a8-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b6a8-134">Request</span></span>
<span data-ttu-id="5b6a8-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

### <a name="response"></a><span data-ttu-id="5b6a8-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b6a8-136">Response</span></span>
<span data-ttu-id="5b6a8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b6a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "value": {
    "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
    "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```




