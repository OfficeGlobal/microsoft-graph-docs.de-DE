---
title: Liste groupPolicyPresentationDecimalTextBoxes
description: Listeneigenschaften und Beziehungen der GroupPolicyPresentationDecimalTextBox-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 45df20c0e7f68ee3939e6d98e7f1a5ddfd3828ba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430017"
---
# <a name="list-grouppolicypresentationdecimaltextboxes"></a><span data-ttu-id="a1347-103">Liste groupPolicyPresentationDecimalTextBoxes</span><span class="sxs-lookup"><span data-stu-id="a1347-103">List groupPolicyPresentationDecimalTextBoxes</span></span>

> <span data-ttu-id="a1347-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a1347-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a1347-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a1347-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1347-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a1347-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1347-107">Listeneigenschaften und Beziehungen der [GroupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="a1347-107">List properties and relationships of the [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1347-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a1347-108">Prerequisites</span></span>
<span data-ttu-id="a1347-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a1347-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a1347-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a1347-111">Permission type</span></span>|<span data-ttu-id="a1347-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a1347-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1347-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a1347-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1347-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1347-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a1347-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a1347-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1347-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1347-116">Not supported.</span></span>|
|<span data-ttu-id="a1347-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a1347-117">Application</span></span>|<span data-ttu-id="a1347-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a1347-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1347-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1347-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="a1347-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a1347-120">Request headers</span></span>
|<span data-ttu-id="a1347-121">Header</span><span class="sxs-lookup"><span data-stu-id="a1347-121">Header</span></span>|<span data-ttu-id="a1347-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a1347-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1347-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="a1347-123">Authorization</span></span>|<span data-ttu-id="a1347-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="a1347-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1347-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a1347-125">Accept</span></span>|<span data-ttu-id="a1347-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1347-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1347-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a1347-127">Request body</span></span>
<span data-ttu-id="a1347-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a1347-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1347-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1347-129">Response</span></span>
<span data-ttu-id="a1347-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [GroupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .</span><span class="sxs-lookup"><span data-stu-id="a1347-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1347-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a1347-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1347-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a1347-132">Request</span></span>
<span data-ttu-id="a1347-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a1347-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

### <a name="response"></a><span data-ttu-id="a1347-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="a1347-134">Response</span></span>
<span data-ttu-id="a1347-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a1347-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 407

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
      "label": "Label value",
      "id": "988daea7-aea7-988d-a7ae-8d98a7ae8d98",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "defaultValue": 12,
      "spin": true,
      "spinStep": 8,
      "required": true,
      "minValue": 8,
      "maxValue": 8
    }
  ]
}
```



