---
title: GroupPolicyPresentationMultiTextBox abrufen
description: Lesen von Eigenschaften und Beziehungen des groupPolicyPresentationMultiTextBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9acc0125f3fc132ea1eb5c1742c56162fe7be391
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148993"
---
# <a name="get-grouppolicypresentationmultitextbox"></a><span data-ttu-id="6544f-103">GroupPolicyPresentationMultiTextBox abrufen</span><span class="sxs-lookup"><span data-stu-id="6544f-103">Get groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="6544f-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6544f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6544f-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="6544f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6544f-106">Lesen von Eigenschaften und Beziehungen des [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6544f-106">Read properties and relationships of the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6544f-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="6544f-107">Prerequisites</span></span>
<span data-ttu-id="6544f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6544f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6544f-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6544f-110">Permission type</span></span>|<span data-ttu-id="6544f-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6544f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6544f-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6544f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6544f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6544f-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6544f-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6544f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6544f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6544f-115">Not supported.</span></span>|
|<span data-ttu-id="6544f-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6544f-116">Application</span></span>|<span data-ttu-id="6544f-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6544f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6544f-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6544f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6544f-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="6544f-119">Optional query parameters</span></span>
<span data-ttu-id="6544f-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6544f-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6544f-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6544f-121">Request headers</span></span>
|<span data-ttu-id="6544f-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6544f-122">Header</span></span>|<span data-ttu-id="6544f-123">Wert</span><span class="sxs-lookup"><span data-stu-id="6544f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6544f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6544f-124">Authorization</span></span>|<span data-ttu-id="6544f-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="6544f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6544f-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="6544f-126">Accept</span></span>|<span data-ttu-id="6544f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6544f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6544f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6544f-128">Request body</span></span>
<span data-ttu-id="6544f-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6544f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6544f-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="6544f-130">Response</span></span>
<span data-ttu-id="6544f-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="6544f-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6544f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6544f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6544f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6544f-133">Request</span></span>
<span data-ttu-id="6544f-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6544f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="6544f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="6544f-135">Response</span></span>
<span data-ttu-id="6544f-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6544f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 311

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
    "label": "Label value",
    "id": "381ac035-c035-381a-35c0-1a3835c01a38",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "required": true,
    "maxLength": 9,
    "maxStrings": 10
  }
}
```




