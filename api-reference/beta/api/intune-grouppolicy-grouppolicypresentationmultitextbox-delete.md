---
title: GroupPolicyPresentationMultiTextBox löschen
description: Löscht eine groupPolicyPresentationMultiTextBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce59d54569771d81fd5a306e3bdf571ab85ea133
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30981048"
---
# <a name="delete-grouppolicypresentationmultitextbox"></a><span data-ttu-id="b6426-103">GroupPolicyPresentationMultiTextBox löschen</span><span class="sxs-lookup"><span data-stu-id="b6426-103">Delete groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="b6426-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b6426-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6426-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b6426-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6426-106">Löscht eine [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span><span class="sxs-lookup"><span data-stu-id="b6426-106">Deletes a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6426-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b6426-107">Prerequisites</span></span>
<span data-ttu-id="b6426-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6426-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b6426-110">Permission type</span></span>|<span data-ttu-id="b6426-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b6426-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6426-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b6426-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6426-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6426-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b6426-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b6426-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6426-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6426-115">Not supported.</span></span>|
|<span data-ttu-id="b6426-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b6426-116">Application</span></span>|<span data-ttu-id="b6426-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b6426-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6426-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6426-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="b6426-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b6426-119">Request headers</span></span>
|<span data-ttu-id="b6426-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b6426-120">Header</span></span>|<span data-ttu-id="b6426-121">Wert</span><span class="sxs-lookup"><span data-stu-id="b6426-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6426-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6426-122">Authorization</span></span>|<span data-ttu-id="b6426-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="b6426-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6426-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="b6426-124">Accept</span></span>|<span data-ttu-id="b6426-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6426-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6426-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b6426-126">Request body</span></span>
<span data-ttu-id="b6426-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b6426-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6426-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6426-128">Response</span></span>
<span data-ttu-id="b6426-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6426-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b6426-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b6426-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6426-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b6426-131">Request</span></span>
<span data-ttu-id="b6426-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b6426-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="b6426-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="b6426-133">Response</span></span>
<span data-ttu-id="b6426-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b6426-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




