---
title: Aktualisieren von „termsAndConditionsAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bd35c13696b910014b6099c1c8f75aa857e28f0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30143050"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="337a0-103">Aktualisieren von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="337a0-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="337a0-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="337a0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="337a0-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="337a0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="337a0-106">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="337a0-106">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="337a0-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="337a0-107">Prerequisites</span></span>
<span data-ttu-id="337a0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="337a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="337a0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="337a0-110">Permission type</span></span>|<span data-ttu-id="337a0-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="337a0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="337a0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="337a0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="337a0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="337a0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="337a0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="337a0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="337a0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="337a0-115">Not supported.</span></span>|
|<span data-ttu-id="337a0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="337a0-116">Application</span></span>|<span data-ttu-id="337a0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="337a0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="337a0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="337a0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="337a0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="337a0-119">Request headers</span></span>
|<span data-ttu-id="337a0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="337a0-120">Header</span></span>|<span data-ttu-id="337a0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="337a0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="337a0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="337a0-122">Authorization</span></span>|<span data-ttu-id="337a0-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="337a0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="337a0-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="337a0-124">Accept</span></span>|<span data-ttu-id="337a0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="337a0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="337a0-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="337a0-126">Request body</span></span>
<span data-ttu-id="337a0-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="337a0-127">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="337a0-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="337a0-128">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="337a0-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="337a0-129">Property</span></span>|<span data-ttu-id="337a0-130">Typ</span><span class="sxs-lookup"><span data-stu-id="337a0-130">Type</span></span>|<span data-ttu-id="337a0-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="337a0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="337a0-132">id</span><span class="sxs-lookup"><span data-stu-id="337a0-132">id</span></span>|<span data-ttu-id="337a0-133">String</span><span class="sxs-lookup"><span data-stu-id="337a0-133">String</span></span>|<span data-ttu-id="337a0-134">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="337a0-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="337a0-135">target</span><span class="sxs-lookup"><span data-stu-id="337a0-135">target</span></span>|[<span data-ttu-id="337a0-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="337a0-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="337a0-137">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="337a0-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="337a0-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="337a0-138">Response</span></span>
<span data-ttu-id="337a0-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="337a0-139">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="337a0-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="337a0-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="337a0-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="337a0-141">Request</span></span>
<span data-ttu-id="337a0-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="337a0-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="337a0-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="337a0-143">Response</span></span>
<span data-ttu-id="337a0-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="337a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




