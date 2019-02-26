---
title: Aktualisieren von „termsAndConditionsAssignment“
description: Diese Methode aktualisiert die Eigenschaften von Objekten des Typs termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8654c7df2f693d8a74bfb993e1274b876eda390e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261852"
---
# <a name="update-termsandconditionsassignment"></a><span data-ttu-id="c79ce-103">Aktualisieren von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="c79ce-103">Update termsAndConditionsAssignment</span></span>

> <span data-ttu-id="c79ce-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c79ce-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c79ce-105">Diese Methode aktualisiert die Eigenschaften von Objekten des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c79ce-105">Update the properties of a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c79ce-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c79ce-106">Prerequisites</span></span>
<span data-ttu-id="c79ce-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c79ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c79ce-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c79ce-109">Permission type</span></span>|<span data-ttu-id="c79ce-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c79ce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c79ce-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c79ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c79ce-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c79ce-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c79ce-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c79ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c79ce-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c79ce-114">Not supported.</span></span>|
|<span data-ttu-id="c79ce-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c79ce-115">Application</span></span>|<span data-ttu-id="c79ce-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c79ce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c79ce-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c79ce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c79ce-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c79ce-118">Request headers</span></span>
|<span data-ttu-id="c79ce-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c79ce-119">Header</span></span>|<span data-ttu-id="c79ce-120">Wert</span><span class="sxs-lookup"><span data-stu-id="c79ce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c79ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c79ce-121">Authorization</span></span>|<span data-ttu-id="c79ce-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c79ce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c79ce-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c79ce-123">Accept</span></span>|<span data-ttu-id="c79ce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c79ce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c79ce-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c79ce-125">Request body</span></span>
<span data-ttu-id="c79ce-126">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) an.</span><span class="sxs-lookup"><span data-stu-id="c79ce-126">In the request body, supply a JSON representation for the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

<span data-ttu-id="c79ce-127">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) erstellen.</span><span class="sxs-lookup"><span data-stu-id="c79ce-127">The following table shows the properties that are required when you create the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span></span>

|<span data-ttu-id="c79ce-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c79ce-128">Property</span></span>|<span data-ttu-id="c79ce-129">Typ</span><span class="sxs-lookup"><span data-stu-id="c79ce-129">Type</span></span>|<span data-ttu-id="c79ce-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c79ce-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c79ce-131">id</span><span class="sxs-lookup"><span data-stu-id="c79ce-131">id</span></span>|<span data-ttu-id="c79ce-132">String</span><span class="sxs-lookup"><span data-stu-id="c79ce-132">String</span></span>|<span data-ttu-id="c79ce-133">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="c79ce-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="c79ce-134">target</span><span class="sxs-lookup"><span data-stu-id="c79ce-134">target</span></span>|[<span data-ttu-id="c79ce-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c79ce-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c79ce-136">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="c79ce-136">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="c79ce-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c79ce-137">Response</span></span>
<span data-ttu-id="c79ce-138">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `200 OK` und ein aktualisiertes Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c79ce-138">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c79ce-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c79ce-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="c79ce-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c79ce-140">Request</span></span>
<span data-ttu-id="c79ce-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c79ce-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
Content-type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="c79ce-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="c79ce-142">Response</span></span>
<span data-ttu-id="c79ce-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c79ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



