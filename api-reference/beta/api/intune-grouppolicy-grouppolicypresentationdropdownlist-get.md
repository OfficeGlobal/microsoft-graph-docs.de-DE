---
title: GroupPolicyPresentationDropdownList abrufen
description: Lesen von Eigenschaften und Beziehungen des groupPolicyPresentationDropdownList-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f514b878eb98a8148df04f9b46ed8d5218c1bbf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142630"
---
# <a name="get-grouppolicypresentationdropdownlist"></a><span data-ttu-id="c4041-103">GroupPolicyPresentationDropdownList abrufen</span><span class="sxs-lookup"><span data-stu-id="c4041-103">Get groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="c4041-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c4041-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4041-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c4041-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4041-106">Lesen von Eigenschaften und Beziehungen des [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c4041-106">Read properties and relationships of the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4041-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c4041-107">Prerequisites</span></span>
<span data-ttu-id="c4041-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c4041-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c4041-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c4041-110">Permission type</span></span>|<span data-ttu-id="c4041-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c4041-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4041-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c4041-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4041-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4041-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c4041-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c4041-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4041-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c4041-115">Not supported.</span></span>|
|<span data-ttu-id="c4041-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c4041-116">Application</span></span>|<span data-ttu-id="c4041-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c4041-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4041-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4041-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4041-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c4041-119">Optional query parameters</span></span>
<span data-ttu-id="c4041-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c4041-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4041-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c4041-121">Request headers</span></span>
|<span data-ttu-id="c4041-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c4041-122">Header</span></span>|<span data-ttu-id="c4041-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c4041-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4041-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4041-124">Authorization</span></span>|<span data-ttu-id="c4041-125">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c4041-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4041-126">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c4041-126">Accept</span></span>|<span data-ttu-id="c4041-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c4041-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4041-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c4041-128">Request body</span></span>
<span data-ttu-id="c4041-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c4041-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4041-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4041-130">Response</span></span>
<span data-ttu-id="c4041-131">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und das [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c4041-131">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4041-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c4041-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4041-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4041-133">Request</span></span>
<span data-ttu-id="c4041-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c4041-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="c4041-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4041-135">Response</span></span>
<span data-ttu-id="c4041-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c4041-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 655

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
    "label": "Label value",
    "id": "ba3ff7c9-f7c9-ba3f-c9f7-3fbac9f73fba",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "defaultItem": {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "Display Name value",
      "value": "Value value"
    },
    "items": [
      {
        "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
        "displayName": "Display Name value",
        "value": "Value value"
      }
    ],
    "required": true
  }
}
```




