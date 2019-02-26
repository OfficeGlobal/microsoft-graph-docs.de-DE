---
title: GroupPolicyPresentationTextBox löschen
description: Löscht eine groupPolicyPresentationTextBox.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e6327a171f2c285ea6b129051593c915a32b434
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152248"
---
# <a name="delete-grouppolicypresentationtextbox"></a><span data-ttu-id="d75ad-103">GroupPolicyPresentationTextBox löschen</span><span class="sxs-lookup"><span data-stu-id="d75ad-103">Delete groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="d75ad-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d75ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d75ad-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d75ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d75ad-106">Löscht eine [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span><span class="sxs-lookup"><span data-stu-id="d75ad-106">Deletes a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d75ad-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d75ad-107">Prerequisites</span></span>
<span data-ttu-id="d75ad-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d75ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d75ad-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d75ad-110">Permission type</span></span>|<span data-ttu-id="d75ad-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d75ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d75ad-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d75ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d75ad-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d75ad-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d75ad-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d75ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d75ad-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d75ad-115">Not supported.</span></span>|
|<span data-ttu-id="d75ad-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d75ad-116">Application</span></span>|<span data-ttu-id="d75ad-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d75ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d75ad-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d75ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="d75ad-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d75ad-119">Request headers</span></span>
|<span data-ttu-id="d75ad-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d75ad-120">Header</span></span>|<span data-ttu-id="d75ad-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d75ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d75ad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d75ad-122">Authorization</span></span>|<span data-ttu-id="d75ad-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d75ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d75ad-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d75ad-124">Accept</span></span>|<span data-ttu-id="d75ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d75ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d75ad-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d75ad-126">Request body</span></span>
<span data-ttu-id="d75ad-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d75ad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d75ad-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="d75ad-128">Response</span></span>
<span data-ttu-id="d75ad-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d75ad-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d75ad-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d75ad-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d75ad-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d75ad-131">Request</span></span>
<span data-ttu-id="d75ad-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d75ad-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="d75ad-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d75ad-133">Response</span></span>
<span data-ttu-id="d75ad-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d75ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




