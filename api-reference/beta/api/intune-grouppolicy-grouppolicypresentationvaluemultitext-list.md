---
title: GroupPolicyPresentationValueMultiTexts aufListen
description: AufListen von Eigenschaften und Beziehungen der groupPolicyPresentationValueMultiText-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5ca53d760e2ab052d13d89caa7ff5c57126ccaa
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162608"
---
# <a name="list-grouppolicypresentationvaluemultitexts"></a><span data-ttu-id="ca272-103">GroupPolicyPresentationValueMultiTexts aufListen</span><span class="sxs-lookup"><span data-stu-id="ca272-103">List groupPolicyPresentationValueMultiTexts</span></span>

> <span data-ttu-id="ca272-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ca272-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca272-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ca272-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca272-106">AufListen von Eigenschaften und Beziehungen der [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="ca272-106">List properties and relationships of the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca272-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ca272-107">Prerequisites</span></span>
<span data-ttu-id="ca272-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ca272-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ca272-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ca272-110">Permission type</span></span>|<span data-ttu-id="ca272-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ca272-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca272-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ca272-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca272-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca272-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ca272-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ca272-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca272-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca272-115">Not supported.</span></span>|
|<span data-ttu-id="ca272-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ca272-116">Application</span></span>|<span data-ttu-id="ca272-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ca272-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca272-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca272-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="ca272-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ca272-119">Request headers</span></span>
|<span data-ttu-id="ca272-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ca272-120">Header</span></span>|<span data-ttu-id="ca272-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ca272-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca272-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca272-122">Authorization</span></span>|<span data-ttu-id="ca272-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ca272-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca272-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ca272-124">Accept</span></span>|<span data-ttu-id="ca272-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca272-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca272-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ca272-126">Request body</span></span>
<span data-ttu-id="ca272-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ca272-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca272-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca272-128">Response</span></span>
<span data-ttu-id="ca272-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ca272-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca272-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ca272-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca272-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ca272-131">Request</span></span>
<span data-ttu-id="ca272-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ca272-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="ca272-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ca272-133">Response</span></span>
<span data-ttu-id="ca272-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ca272-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 353

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "id": "5156903b-903b-5156-3b90-56513b905651",
      "values": [
        "Values value"
      ]
    }
  ]
}
```




