---
title: Erstellen von termsAndConditionsGroupAssignment
description: Erstellen eines neuen TermsAndConditionsGroupAssignment-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 669715f6d6a000978ba8918c08d0e1ea9446b86b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963766"
---
# <a name="create-termsandconditionsgroupassignment"></a><span data-ttu-id="fd35b-103">Erstellen von termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="fd35b-103">Create termsAndConditionsGroupAssignment</span></span>

> <span data-ttu-id="fd35b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fd35b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd35b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fd35b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd35b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="fd35b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd35b-107">Erstellen eines neuen [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fd35b-107">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd35b-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fd35b-108">Prerequisites</span></span>
<span data-ttu-id="fd35b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd35b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd35b-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd35b-111">Permission type</span></span>|<span data-ttu-id="fd35b-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd35b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd35b-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd35b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fd35b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd35b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fd35b-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd35b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd35b-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd35b-116">Not supported.</span></span>|
|<span data-ttu-id="fd35b-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd35b-117">Application</span></span>|<span data-ttu-id="fd35b-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd35b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd35b-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd35b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="fd35b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd35b-120">Request headers</span></span>
|<span data-ttu-id="fd35b-121">Header</span><span class="sxs-lookup"><span data-stu-id="fd35b-121">Header</span></span>|<span data-ttu-id="fd35b-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fd35b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd35b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd35b-123">Authorization</span></span>|<span data-ttu-id="fd35b-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fd35b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd35b-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fd35b-125">Accept</span></span>|<span data-ttu-id="fd35b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd35b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd35b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd35b-127">Request body</span></span>
<span data-ttu-id="fd35b-128">Geben Sie im Textkörper Anforderung für das Objekt TermsAndConditionsGroupAssignment eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="fd35b-128">In the request body, supply a JSON representation for the termsAndConditionsGroupAssignment object.</span></span>

<span data-ttu-id="fd35b-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die TermsAndConditionsGroupAssignment erstellen.</span><span class="sxs-lookup"><span data-stu-id="fd35b-129">The following table shows the properties that are required when you create the termsAndConditionsGroupAssignment.</span></span>

|<span data-ttu-id="fd35b-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fd35b-130">Property</span></span>|<span data-ttu-id="fd35b-131">Typ</span><span class="sxs-lookup"><span data-stu-id="fd35b-131">Type</span></span>|<span data-ttu-id="fd35b-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd35b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd35b-133">id</span><span class="sxs-lookup"><span data-stu-id="fd35b-133">id</span></span>|<span data-ttu-id="fd35b-134">String</span><span class="sxs-lookup"><span data-stu-id="fd35b-134">String</span></span>|<span data-ttu-id="fd35b-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="fd35b-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="fd35b-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="fd35b-136">targetGroupId</span></span>|<span data-ttu-id="fd35b-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fd35b-137">String</span></span>|<span data-ttu-id="fd35b-138">Eindeutiger Bezeichner der einer Gruppe, der die Richtlinie T & C zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="fd35b-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="fd35b-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd35b-139">Response</span></span>
<span data-ttu-id="fd35b-140">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="fd35b-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd35b-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd35b-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd35b-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd35b-142">Request</span></span>
<span data-ttu-id="fd35b-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd35b-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="fd35b-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd35b-144">Response</span></span>
<span data-ttu-id="fd35b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd35b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```





