---
title: Aktualisieren von „termsAndConditionsAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a808ebfcce08fc93c8d5f95b11a43aea742b4b08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955443"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="bd94d-103">Aktualisieren von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="bd94d-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="bd94d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bd94d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd94d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bd94d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd94d-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bd94d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bd94d-107">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bd94d-107">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bd94d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bd94d-108">Prerequisites</span></span>
<span data-ttu-id="bd94d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd94d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd94d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bd94d-111">Permission type</span></span>|<span data-ttu-id="bd94d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bd94d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd94d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bd94d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd94d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd94d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bd94d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bd94d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd94d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd94d-116">Not supported.</span></span>|
|<span data-ttu-id="bd94d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bd94d-117">Application</span></span>|<span data-ttu-id="bd94d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bd94d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd94d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd94d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="bd94d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bd94d-120">Request headers</span></span>
|<span data-ttu-id="bd94d-121">Header</span><span class="sxs-lookup"><span data-stu-id="bd94d-121">Header</span></span>|<span data-ttu-id="bd94d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bd94d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd94d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd94d-123">Authorization</span></span>|<span data-ttu-id="bd94d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bd94d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd94d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bd94d-125">Accept</span></span>|<span data-ttu-id="bd94d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd94d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd94d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bd94d-127">Request body</span></span>
<span data-ttu-id="bd94d-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="bd94d-128">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="bd94d-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="bd94d-129">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="bd94d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bd94d-130">Property</span></span>|<span data-ttu-id="bd94d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bd94d-131">Type</span></span>|<span data-ttu-id="bd94d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bd94d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd94d-133">id</span><span class="sxs-lookup"><span data-stu-id="bd94d-133">id</span></span>|<span data-ttu-id="bd94d-134">String</span><span class="sxs-lookup"><span data-stu-id="bd94d-134">String</span></span>|<span data-ttu-id="bd94d-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="bd94d-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="bd94d-136">target</span><span class="sxs-lookup"><span data-stu-id="bd94d-136">target</span></span>|[<span data-ttu-id="bd94d-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bd94d-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bd94d-138">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="bd94d-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="bd94d-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd94d-139">Response</span></span>
<span data-ttu-id="bd94d-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="bd94d-140">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd94d-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bd94d-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="bd94d-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bd94d-142">Request</span></span>
<span data-ttu-id="bd94d-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bd94d-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="bd94d-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="bd94d-144">Response</span></span>
<span data-ttu-id="bd94d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bd94d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 217

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





