---
title: GroupPolicyPresentationDropdownList löschen
description: Löscht eine GroupPolicyPresentationDropdownList.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d7f9f4d26f14ab0bcd2ae01fa405aef03a63139
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430107"
---
# <a name="delete-grouppolicypresentationdropdownlist"></a><span data-ttu-id="20f91-103">GroupPolicyPresentationDropdownList löschen</span><span class="sxs-lookup"><span data-stu-id="20f91-103">Delete groupPolicyPresentationDropdownList</span></span>

> <span data-ttu-id="20f91-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="20f91-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="20f91-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="20f91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20f91-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="20f91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20f91-107">Löscht eine [GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span><span class="sxs-lookup"><span data-stu-id="20f91-107">Deletes a [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20f91-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="20f91-108">Prerequisites</span></span>
<span data-ttu-id="20f91-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="20f91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="20f91-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="20f91-111">Permission type</span></span>|<span data-ttu-id="20f91-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="20f91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20f91-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="20f91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20f91-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20f91-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="20f91-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="20f91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20f91-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20f91-116">Not supported.</span></span>|
|<span data-ttu-id="20f91-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="20f91-117">Application</span></span>|<span data-ttu-id="20f91-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="20f91-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20f91-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="20f91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
DELETE /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="20f91-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="20f91-120">Request headers</span></span>
|<span data-ttu-id="20f91-121">Header</span><span class="sxs-lookup"><span data-stu-id="20f91-121">Header</span></span>|<span data-ttu-id="20f91-122">Wert</span><span class="sxs-lookup"><span data-stu-id="20f91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20f91-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="20f91-123">Authorization</span></span>|<span data-ttu-id="20f91-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="20f91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20f91-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="20f91-125">Accept</span></span>|<span data-ttu-id="20f91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20f91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20f91-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="20f91-127">Request body</span></span>
<span data-ttu-id="20f91-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="20f91-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20f91-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="20f91-129">Response</span></span>
<span data-ttu-id="20f91-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="20f91-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="20f91-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="20f91-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="20f91-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="20f91-132">Request</span></span>
<span data-ttu-id="20f91-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="20f91-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
```

### <a name="response"></a><span data-ttu-id="20f91-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="20f91-134">Response</span></span>
<span data-ttu-id="20f91-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="20f91-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




