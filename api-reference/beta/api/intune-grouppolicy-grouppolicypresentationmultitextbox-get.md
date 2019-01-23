---
title: Abrufen von groupPolicyPresentationMultiTextBox
description: Lesen Sie Eigenschaften und Beziehungen des GroupPolicyPresentationMultiTextBox-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2830b40bf9456f52a02cc57c2b5ebd47d5e89d28
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429938"
---
# <a name="get-grouppolicypresentationmultitextbox"></a><span data-ttu-id="66cb6-103">Abrufen von groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="66cb6-103">Get groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="66cb6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="66cb6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="66cb6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="66cb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66cb6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="66cb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66cb6-107">Lesen Sie Eigenschaften und Beziehungen des [GroupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="66cb6-107">Read properties and relationships of the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66cb6-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="66cb6-108">Prerequisites</span></span>
<span data-ttu-id="66cb6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="66cb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="66cb6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66cb6-111">Permission type</span></span>|<span data-ttu-id="66cb6-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="66cb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66cb6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66cb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="66cb6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="66cb6-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="66cb6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="66cb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66cb6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66cb6-116">Not supported.</span></span>|
|<span data-ttu-id="66cb6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66cb6-117">Application</span></span>|<span data-ttu-id="66cb6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="66cb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66cb6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66cb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="66cb6-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="66cb6-120">Optional query parameters</span></span>
<span data-ttu-id="66cb6-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://docs.microsoft.com/en-us/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="66cb6-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66cb6-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66cb6-122">Request headers</span></span>
|<span data-ttu-id="66cb6-123">Header</span><span class="sxs-lookup"><span data-stu-id="66cb6-123">Header</span></span>|<span data-ttu-id="66cb6-124">Wert</span><span class="sxs-lookup"><span data-stu-id="66cb6-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66cb6-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="66cb6-125">Authorization</span></span>|<span data-ttu-id="66cb6-126">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="66cb6-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66cb6-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="66cb6-127">Accept</span></span>|<span data-ttu-id="66cb6-128">application/json</span><span class="sxs-lookup"><span data-stu-id="66cb6-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66cb6-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66cb6-129">Request body</span></span>
<span data-ttu-id="66cb6-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="66cb6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66cb6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="66cb6-131">Response</span></span>
<span data-ttu-id="66cb6-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [GroupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="66cb6-132">If successful, this method returns a `200 OK` response code and [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66cb6-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66cb6-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="66cb6-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66cb6-134">Request</span></span>
<span data-ttu-id="66cb6-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66cb6-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="66cb6-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="66cb6-136">Response</span></span>
<span data-ttu-id="66cb6-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66cb6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




