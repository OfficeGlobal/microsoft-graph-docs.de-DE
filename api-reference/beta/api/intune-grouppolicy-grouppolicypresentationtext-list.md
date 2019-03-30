---
title: GroupPolicyPresentationTexts aufListen
description: AufListen von Eigenschaften und Beziehungen der groupPolicyPresentationText-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c0f63088db3428b0f031a1074d9233fba9e04231
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977170"
---
# <a name="list-grouppolicypresentationtexts"></a><span data-ttu-id="b98cb-103">GroupPolicyPresentationTexts aufListen</span><span class="sxs-lookup"><span data-stu-id="b98cb-103">List groupPolicyPresentationTexts</span></span>

> <span data-ttu-id="b98cb-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b98cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b98cb-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b98cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b98cb-106">AufListen von Eigenschaften und Beziehungen der [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="b98cb-106">List properties and relationships of the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b98cb-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b98cb-107">Prerequisites</span></span>
<span data-ttu-id="b98cb-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b98cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b98cb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b98cb-110">Permission type</span></span>|<span data-ttu-id="b98cb-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b98cb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b98cb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b98cb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b98cb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b98cb-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b98cb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b98cb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b98cb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b98cb-115">Not supported.</span></span>|
|<span data-ttu-id="b98cb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b98cb-116">Application</span></span>|<span data-ttu-id="b98cb-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b98cb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b98cb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b98cb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="b98cb-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b98cb-119">Request headers</span></span>
|<span data-ttu-id="b98cb-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b98cb-120">Header</span></span>|<span data-ttu-id="b98cb-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b98cb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b98cb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b98cb-122">Authorization</span></span>|<span data-ttu-id="b98cb-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b98cb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b98cb-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b98cb-124">Accept</span></span>|<span data-ttu-id="b98cb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b98cb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b98cb-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b98cb-126">Request body</span></span>
<span data-ttu-id="b98cb-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b98cb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b98cb-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b98cb-128">Response</span></span>
<span data-ttu-id="b98cb-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="b98cb-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b98cb-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b98cb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b98cb-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b98cb-131">Request</span></span>
<span data-ttu-id="b98cb-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b98cb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="b98cb-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b98cb-133">Response</span></span>
<span data-ttu-id="b98cb-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b98cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 258

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
      "label": "Label value",
      "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```




