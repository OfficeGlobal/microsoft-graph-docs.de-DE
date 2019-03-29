---
title: GroupPolicyPresentationDropdownLists aufListen
description: AufListen von Eigenschaften und Beziehungen der groupPolicyPresentationDropdownList-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58f9f524b177396b5ddf712919183d226e3c78d4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971927"
---
# <a name="list-grouppolicypresentationdropdownlists"></a><span data-ttu-id="22782-103">GroupPolicyPresentationDropdownLists aufListen</span><span class="sxs-lookup"><span data-stu-id="22782-103">List groupPolicyPresentationDropdownLists</span></span>

> <span data-ttu-id="22782-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="22782-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22782-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="22782-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22782-106">AufListen von Eigenschaften und Beziehungen der [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="22782-106">List properties and relationships of the [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22782-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="22782-107">Prerequisites</span></span>
<span data-ttu-id="22782-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22782-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22782-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="22782-110">Permission type</span></span>|<span data-ttu-id="22782-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="22782-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22782-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="22782-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22782-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="22782-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="22782-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="22782-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22782-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22782-115">Not supported.</span></span>|
|<span data-ttu-id="22782-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="22782-116">Application</span></span>|<span data-ttu-id="22782-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="22782-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22782-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="22782-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="22782-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="22782-119">Request headers</span></span>
|<span data-ttu-id="22782-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="22782-120">Header</span></span>|<span data-ttu-id="22782-121">Wert</span><span class="sxs-lookup"><span data-stu-id="22782-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22782-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22782-122">Authorization</span></span>|<span data-ttu-id="22782-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="22782-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22782-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="22782-124">Accept</span></span>|<span data-ttu-id="22782-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22782-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22782-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="22782-126">Request body</span></span>
<span data-ttu-id="22782-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="22782-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22782-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="22782-128">Response</span></span>
<span data-ttu-id="22782-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="22782-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22782-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="22782-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="22782-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="22782-131">Request</span></span>
<span data-ttu-id="22782-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="22782-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="22782-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="22782-133">Response</span></span>
<span data-ttu-id="22782-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="22782-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 703

{
  "value": [
    {
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
  ]
}
```




