---
title: GroupPolicyPresentationTexts aufListen
description: AufListen von Eigenschaften und Beziehungen der groupPolicyPresentationText-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1aebda7816b3198620ffe0c6a98232f0accd55f2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152003"
---
# <a name="list-grouppolicypresentationtexts"></a><span data-ttu-id="0ce41-103">GroupPolicyPresentationTexts aufListen</span><span class="sxs-lookup"><span data-stu-id="0ce41-103">List groupPolicyPresentationTexts</span></span>

> <span data-ttu-id="0ce41-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0ce41-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ce41-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0ce41-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ce41-106">AufListen von Eigenschaften und Beziehungen der [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="0ce41-106">List properties and relationships of the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ce41-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0ce41-107">Prerequisites</span></span>
<span data-ttu-id="0ce41-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ce41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0ce41-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0ce41-110">Permission type</span></span>|<span data-ttu-id="0ce41-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0ce41-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ce41-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0ce41-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ce41-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ce41-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0ce41-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0ce41-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ce41-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ce41-115">Not supported.</span></span>|
|<span data-ttu-id="0ce41-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0ce41-116">Application</span></span>|<span data-ttu-id="0ce41-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0ce41-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ce41-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ce41-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="0ce41-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0ce41-119">Request headers</span></span>
|<span data-ttu-id="0ce41-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0ce41-120">Header</span></span>|<span data-ttu-id="0ce41-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0ce41-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ce41-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ce41-122">Authorization</span></span>|<span data-ttu-id="0ce41-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0ce41-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ce41-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0ce41-124">Accept</span></span>|<span data-ttu-id="0ce41-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ce41-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ce41-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0ce41-126">Request body</span></span>
<span data-ttu-id="0ce41-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0ce41-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ce41-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ce41-128">Response</span></span>
<span data-ttu-id="0ce41-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0ce41-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ce41-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0ce41-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ce41-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0ce41-131">Request</span></span>
<span data-ttu-id="0ce41-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0ce41-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="0ce41-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="0ce41-133">Response</span></span>
<span data-ttu-id="0ce41-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0ce41-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




