---
title: Erstellen von „termsAndConditionsAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs termsAndConditionsAssignment.
ms.openlocfilehash: cae5456635c9e05546f885062d84b8660ad12d3b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061207"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="376d2-103">Erstellen von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="376d2-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="376d2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="376d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="376d2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="376d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="376d2-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="376d2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="376d2-107">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="376d2-107">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="376d2-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="376d2-108">Prerequisites</span></span>
<span data-ttu-id="376d2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="376d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="376d2-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="376d2-111">Permission type</span></span>|<span data-ttu-id="376d2-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="376d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="376d2-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="376d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="376d2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="376d2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="376d2-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="376d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="376d2-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="376d2-116">Not supported.</span></span>|
|<span data-ttu-id="376d2-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="376d2-117">Application</span></span>|<span data-ttu-id="376d2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="376d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="376d2-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="376d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="376d2-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="376d2-120">Request headers</span></span>
|<span data-ttu-id="376d2-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="376d2-121">Header</span></span>|<span data-ttu-id="376d2-122">Wert</span><span class="sxs-lookup"><span data-stu-id="376d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="376d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="376d2-123">Authorization</span></span>|<span data-ttu-id="376d2-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="376d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="376d2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="376d2-125">Accept</span></span>|<span data-ttu-id="376d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="376d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="376d2-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="376d2-127">Request body</span></span>
<span data-ttu-id="376d2-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditionsAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="376d2-128">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="376d2-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditionsAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="376d2-129">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="376d2-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="376d2-130">Property</span></span>|<span data-ttu-id="376d2-131">Typ</span><span class="sxs-lookup"><span data-stu-id="376d2-131">Type</span></span>|<span data-ttu-id="376d2-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="376d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="376d2-133">id</span><span class="sxs-lookup"><span data-stu-id="376d2-133">id</span></span>|<span data-ttu-id="376d2-134">String</span><span class="sxs-lookup"><span data-stu-id="376d2-134">String</span></span>|<span data-ttu-id="376d2-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="376d2-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="376d2-136">target</span><span class="sxs-lookup"><span data-stu-id="376d2-136">target</span></span>|[<span data-ttu-id="376d2-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="376d2-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="376d2-138">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="376d2-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="376d2-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="376d2-139">Response</span></span>
<span data-ttu-id="376d2-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="376d2-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="376d2-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="376d2-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="376d2-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="376d2-142">Request</span></span>
<span data-ttu-id="376d2-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="376d2-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="376d2-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="376d2-144">Response</span></span>
<span data-ttu-id="376d2-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="376d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




