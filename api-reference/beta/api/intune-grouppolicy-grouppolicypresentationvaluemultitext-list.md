---
title: Liste groupPolicyPresentationValueMultiTexts
description: Listeneigenschaften und Beziehungen der GroupPolicyPresentationValueMultiText-Objekte.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4c2516b76e9de24e068a08771380f6bea74035c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428888"
---
# <a name="list-grouppolicypresentationvaluemultitexts"></a><span data-ttu-id="556b8-103">Liste groupPolicyPresentationValueMultiTexts</span><span class="sxs-lookup"><span data-stu-id="556b8-103">List groupPolicyPresentationValueMultiTexts</span></span>

> <span data-ttu-id="556b8-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="556b8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="556b8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="556b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="556b8-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="556b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="556b8-107">Listeneigenschaften und Beziehungen der [GroupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) -Objekte.</span><span class="sxs-lookup"><span data-stu-id="556b8-107">List properties and relationships of the [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="556b8-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="556b8-108">Prerequisites</span></span>
<span data-ttu-id="556b8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="556b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="556b8-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="556b8-111">Permission type</span></span>|<span data-ttu-id="556b8-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="556b8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="556b8-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="556b8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="556b8-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="556b8-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="556b8-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="556b8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="556b8-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="556b8-116">Not supported.</span></span>|
|<span data-ttu-id="556b8-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="556b8-117">Application</span></span>|<span data-ttu-id="556b8-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="556b8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="556b8-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="556b8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

## <a name="request-headers"></a><span data-ttu-id="556b8-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="556b8-120">Request headers</span></span>
|<span data-ttu-id="556b8-121">Header</span><span class="sxs-lookup"><span data-stu-id="556b8-121">Header</span></span>|<span data-ttu-id="556b8-122">Wert</span><span class="sxs-lookup"><span data-stu-id="556b8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="556b8-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="556b8-123">Authorization</span></span>|<span data-ttu-id="556b8-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="556b8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="556b8-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="556b8-125">Accept</span></span>|<span data-ttu-id="556b8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="556b8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="556b8-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="556b8-127">Request body</span></span>
<span data-ttu-id="556b8-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="556b8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="556b8-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="556b8-129">Response</span></span>
<span data-ttu-id="556b8-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [GroupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) .</span><span class="sxs-lookup"><span data-stu-id="556b8-130">If successful, this method returns a `200 OK` response code and a collection of [groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="556b8-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="556b8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="556b8-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="556b8-132">Request</span></span>
<span data-ttu-id="556b8-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="556b8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues
```

### <a name="response"></a><span data-ttu-id="556b8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="556b8-134">Response</span></span>
<span data-ttu-id="556b8-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="556b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




