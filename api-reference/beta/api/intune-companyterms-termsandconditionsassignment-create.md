---
title: Erstellen von „termsAndConditionsAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d114a55da1c55a1aa7c37b969b2072410f7bbc16
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141734"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="483be-103">Erstellen von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="483be-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="483be-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="483be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="483be-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="483be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="483be-106">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="483be-106">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="483be-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="483be-107">Prerequisites</span></span>
<span data-ttu-id="483be-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="483be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="483be-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="483be-110">Permission type</span></span>|<span data-ttu-id="483be-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="483be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="483be-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="483be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="483be-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="483be-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="483be-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="483be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="483be-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="483be-115">Not supported.</span></span>|
|<span data-ttu-id="483be-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="483be-116">Application</span></span>|<span data-ttu-id="483be-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="483be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="483be-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="483be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="483be-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="483be-119">Request headers</span></span>
|<span data-ttu-id="483be-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="483be-120">Header</span></span>|<span data-ttu-id="483be-121">Wert</span><span class="sxs-lookup"><span data-stu-id="483be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="483be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="483be-122">Authorization</span></span>|<span data-ttu-id="483be-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="483be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="483be-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="483be-124">Accept</span></span>|<span data-ttu-id="483be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="483be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="483be-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="483be-126">Request body</span></span>
<span data-ttu-id="483be-127">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditionsAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="483be-127">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="483be-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditionsAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="483be-128">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="483be-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="483be-129">Property</span></span>|<span data-ttu-id="483be-130">Typ</span><span class="sxs-lookup"><span data-stu-id="483be-130">Type</span></span>|<span data-ttu-id="483be-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="483be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="483be-132">id</span><span class="sxs-lookup"><span data-stu-id="483be-132">id</span></span>|<span data-ttu-id="483be-133">String</span><span class="sxs-lookup"><span data-stu-id="483be-133">String</span></span>|<span data-ttu-id="483be-134">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="483be-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="483be-135">target</span><span class="sxs-lookup"><span data-stu-id="483be-135">target</span></span>|[<span data-ttu-id="483be-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="483be-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="483be-137">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="483be-137">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="483be-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="483be-138">Response</span></span>
<span data-ttu-id="483be-139">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="483be-139">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="483be-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="483be-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="483be-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="483be-141">Request</span></span>
<span data-ttu-id="483be-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="483be-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="483be-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="483be-143">Response</span></span>
<span data-ttu-id="483be-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="483be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




