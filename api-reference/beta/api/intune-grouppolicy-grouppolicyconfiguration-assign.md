---
title: Aktion „assign“
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 06b96d793c07ba5fd3bc776d4b389c77708c8519
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430016"
---
# <a name="assign-action"></a><span data-ttu-id="4d592-103">Aktion „assign“</span><span class="sxs-lookup"><span data-stu-id="4d592-103">assign action</span></span>

> <span data-ttu-id="4d592-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="4d592-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4d592-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4d592-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4d592-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d592-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d592-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4d592-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4d592-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="4d592-108">Prerequisites</span></span>
<span data-ttu-id="4d592-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4d592-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4d592-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d592-111">Permission type</span></span>|<span data-ttu-id="4d592-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d592-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d592-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d592-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4d592-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d592-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4d592-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d592-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d592-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d592-116">Not supported.</span></span>|
|<span data-ttu-id="4d592-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d592-117">Application</span></span>|<span data-ttu-id="4d592-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d592-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d592-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d592-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4d592-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d592-120">Request headers</span></span>
|<span data-ttu-id="4d592-121">Header</span><span class="sxs-lookup"><span data-stu-id="4d592-121">Header</span></span>|<span data-ttu-id="4d592-122">Wert</span><span class="sxs-lookup"><span data-stu-id="4d592-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d592-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4d592-123">Authorization</span></span>|<span data-ttu-id="4d592-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="4d592-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d592-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="4d592-125">Accept</span></span>|<span data-ttu-id="4d592-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d592-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d592-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d592-127">Request body</span></span>
<span data-ttu-id="4d592-128">Geben Sie als Anforderungstext eine JSON-Darstellung der Parameter an.</span><span class="sxs-lookup"><span data-stu-id="4d592-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4d592-129">In der folgenden Tabelle sind die Parameter aufgeführt, die mit dieser Aktion verwendet werden können.</span><span class="sxs-lookup"><span data-stu-id="4d592-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4d592-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4d592-130">Property</span></span>|<span data-ttu-id="4d592-131">Typ</span><span class="sxs-lookup"><span data-stu-id="4d592-131">Type</span></span>|<span data-ttu-id="4d592-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d592-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d592-133">assignments</span><span class="sxs-lookup"><span data-stu-id="4d592-133">assignments</span></span>|<span data-ttu-id="4d592-134">[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="4d592-134">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4d592-135">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="4d592-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4d592-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d592-136">Response</span></span>
<span data-ttu-id="4d592-137">Wenn erfolgreich ist, diese Aktion gibt eine `200 OK` Antwortcode und eine [GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Auflistung im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4d592-137">If successful, this action returns a `200 OK` response code and a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d592-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d592-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d592-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d592-139">Request</span></span>
<span data-ttu-id="4d592-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d592-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assign

Content-type: application/json
Content-length: 350

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4d592-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d592-141">Response</span></span>
<span data-ttu-id="4d592-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d592-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
      "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```




