---
title: GroupPolicyPresentationValueMultiText abrufen
description: Lesen von Eigenschaften und Beziehungen des groupPolicyPresentationValueMultiText-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3beb8654c55424b98ba588cf20bc8bf22c7f778e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152241"
---
# <a name="get-grouppolicypresentationvaluemultitext"></a><span data-ttu-id="818e0-103">GroupPolicyPresentationValueMultiText abrufen</span><span class="sxs-lookup"><span data-stu-id="818e0-103">Get groupPolicyPresentationValueMultiText</span></span>

> <span data-ttu-id="818e0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="818e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="818e0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="818e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="818e0-106">Lesen von Eigenschaften und Beziehungen des [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="818e0-106">Read properties and relationships of the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="818e0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="818e0-107">Prerequisites</span></span>
<span data-ttu-id="818e0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="818e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="818e0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="818e0-110">Permission type</span></span>|<span data-ttu-id="818e0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="818e0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="818e0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="818e0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="818e0-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="818e0-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="818e0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="818e0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="818e0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="818e0-115">Not supported.</span></span>|
|<span data-ttu-id="818e0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="818e0-116">Application</span></span>|<span data-ttu-id="818e0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="818e0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="818e0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="818e0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="818e0-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="818e0-119">Optional query parameters</span></span>
<span data-ttu-id="818e0-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="818e0-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="818e0-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="818e0-121">Request headers</span></span>
|<span data-ttu-id="818e0-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="818e0-122">Header</span></span>|<span data-ttu-id="818e0-123">Wert</span><span class="sxs-lookup"><span data-stu-id="818e0-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="818e0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="818e0-124">Authorization</span></span>|<span data-ttu-id="818e0-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="818e0-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="818e0-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="818e0-126">Accept</span></span>|<span data-ttu-id="818e0-127">application/json</span><span class="sxs-lookup"><span data-stu-id="818e0-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="818e0-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="818e0-128">Request body</span></span>
<span data-ttu-id="818e0-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="818e0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="818e0-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="818e0-130">Response</span></span>
<span data-ttu-id="818e0-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="818e0-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="818e0-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="818e0-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="818e0-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="818e0-133">Request</span></span>
<span data-ttu-id="818e0-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="818e0-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

### <a name="response"></a><span data-ttu-id="818e0-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="818e0-135">Response</span></span>
<span data-ttu-id="818e0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="818e0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 325

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "id": "5156903b-903b-5156-3b90-56513b905651",
    "values": [
      "Values value"
    ]
  }
}
```




