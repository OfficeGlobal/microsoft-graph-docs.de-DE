---
title: OfficeClientConfigurationAssignment abrufen
description: Lesen von Eigenschaften und Beziehungen des officeClientConfigurationAssignment-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6cf3416b606fc1fa32d3657ef77317834980a046
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146690"
---
# <a name="get-officeclientconfigurationassignment"></a><span data-ttu-id="c8514-103">OfficeClientConfigurationAssignment abrufen</span><span class="sxs-lookup"><span data-stu-id="c8514-103">Get officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="c8514-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c8514-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8514-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c8514-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8514-106">Lesen von Eigenschaften und Beziehungen des [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c8514-106">Read properties and relationships of the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8514-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c8514-107">Prerequisites</span></span>
<span data-ttu-id="c8514-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8514-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8514-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c8514-110">Permission type</span></span>|<span data-ttu-id="c8514-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c8514-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8514-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c8514-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c8514-113">\* \* TODO: Bestimmen von Bereichen \* \*</span><span class="sxs-lookup"><span data-stu-id="c8514-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="c8514-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c8514-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8514-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8514-115">Not supported.</span></span>|
|<span data-ttu-id="c8514-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c8514-116">Application</span></span>|<span data-ttu-id="c8514-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c8514-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8514-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8514-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8514-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c8514-119">Optional query parameters</span></span>
<span data-ttu-id="c8514-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c8514-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c8514-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c8514-121">Request headers</span></span>
|<span data-ttu-id="c8514-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c8514-122">Header</span></span>|<span data-ttu-id="c8514-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c8514-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8514-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8514-124">Authorization</span></span>|<span data-ttu-id="c8514-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c8514-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8514-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c8514-126">Accept</span></span>|<span data-ttu-id="c8514-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c8514-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8514-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c8514-128">Request body</span></span>
<span data-ttu-id="c8514-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c8514-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8514-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8514-130">Response</span></span>
<span data-ttu-id="c8514-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c8514-131">If successful, this method returns a `200 OK` response code and [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8514-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c8514-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8514-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c8514-133">Request</span></span>
<span data-ttu-id="c8514-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c8514-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c8514-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c8514-135">Response</span></span>
<span data-ttu-id="c8514-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c8514-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": {
    "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
    "id": "804730f3-30f3-8047-f330-4780f3304780",
    "target": {
      "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
    }
  }
}
```



