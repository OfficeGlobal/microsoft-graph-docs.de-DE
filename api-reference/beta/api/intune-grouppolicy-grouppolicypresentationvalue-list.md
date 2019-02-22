---
title: GroupPolicyPresentationValues aufListen
description: AufListen von Eigenschaften und Beziehungen der groupPolicyPresentationValue-Objekte.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3958e5b7cf03fc420f7b6c88cacba19d02142722
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152318"
---
# <a name="list-grouppolicypresentationvalues"></a><span data-ttu-id="ae920-103">GroupPolicyPresentationValues aufListen</span><span class="sxs-lookup"><span data-stu-id="ae920-103">List groupPolicyPresentationValues</span></span>

> <span data-ttu-id="ae920-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ae920-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae920-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="ae920-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae920-106">AufListen von Eigenschaften und Beziehungen der [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="ae920-106">List properties and relationships of the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae920-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="ae920-107">Prerequisites</span></span>
<span data-ttu-id="ae920-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ae920-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae920-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ae920-110">Permission type</span></span>|<span data-ttu-id="ae920-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ae920-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae920-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ae920-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae920-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae920-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ae920-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ae920-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae920-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae920-115">Not supported.</span></span>|
|<span data-ttu-id="ae920-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ae920-116">Application</span></span>|<span data-ttu-id="ae920-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ae920-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae920-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae920-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="ae920-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ae920-119">Request headers</span></span>
|<span data-ttu-id="ae920-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ae920-120">Header</span></span>|<span data-ttu-id="ae920-121">Wert</span><span class="sxs-lookup"><span data-stu-id="ae920-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae920-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae920-122">Authorization</span></span>|<span data-ttu-id="ae920-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="ae920-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae920-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="ae920-124">Accept</span></span>|<span data-ttu-id="ae920-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae920-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae920-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ae920-126">Request body</span></span>
<span data-ttu-id="ae920-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ae920-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae920-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae920-128">Response</span></span>
<span data-ttu-id="ae920-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ae920-129">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae920-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ae920-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae920-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ae920-131">Request</span></span>
<span data-ttu-id="ae920-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ae920-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="ae920-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ae920-133">Response</span></span>
<span data-ttu-id="ae920-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ae920-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "id": "8132eaab-eaab-8132-abea-3281abea3281"
    }
  ]
}
```




