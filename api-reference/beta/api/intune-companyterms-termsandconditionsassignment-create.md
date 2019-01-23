---
title: Erstellen von „termsAndConditionsAssignment“
description: Diese Methode erstellt ein neues Objekt des Typs termsAndConditionsAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fe83995c1a0d7af5e3f0e2eea88813b7c490ba2a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398058"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="9f575-103">Erstellen von „termsAndConditionsAssignment“</span><span class="sxs-lookup"><span data-stu-id="9f575-103">Create termsAndConditionsAssignment</span></span>

> <span data-ttu-id="9f575-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="9f575-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9f575-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9f575-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f575-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f575-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f575-107">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9f575-107">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f575-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9f575-108">Prerequisites</span></span>
<span data-ttu-id="9f575-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f575-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9f575-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f575-111">Permission type</span></span>|<span data-ttu-id="9f575-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f575-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f575-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f575-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f575-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f575-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f575-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f575-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f575-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f575-116">Not supported.</span></span>|
|<span data-ttu-id="9f575-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f575-117">Application</span></span>|<span data-ttu-id="9f575-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f575-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f575-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f575-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9f575-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f575-120">Request headers</span></span>
|<span data-ttu-id="9f575-121">Header</span><span class="sxs-lookup"><span data-stu-id="9f575-121">Header</span></span>|<span data-ttu-id="9f575-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9f575-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f575-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="9f575-123">Authorization</span></span>|<span data-ttu-id="9f575-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9f575-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f575-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="9f575-125">Accept</span></span>|<span data-ttu-id="9f575-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f575-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f575-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f575-127">Request body</span></span>
<span data-ttu-id="9f575-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditionsAssignment“ an.</span><span class="sxs-lookup"><span data-stu-id="9f575-128">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="9f575-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditionsAssignment“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="9f575-129">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="9f575-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9f575-130">Property</span></span>|<span data-ttu-id="9f575-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9f575-131">Type</span></span>|<span data-ttu-id="9f575-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f575-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f575-133">id</span><span class="sxs-lookup"><span data-stu-id="9f575-133">id</span></span>|<span data-ttu-id="9f575-134">String</span><span class="sxs-lookup"><span data-stu-id="9f575-134">String</span></span>|<span data-ttu-id="9f575-135">Eindeutiger Bezeichner der Entität</span><span class="sxs-lookup"><span data-stu-id="9f575-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="9f575-136">target</span><span class="sxs-lookup"><span data-stu-id="9f575-136">target</span></span>|[<span data-ttu-id="9f575-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9f575-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9f575-138">Zuweisungsziel, dem die Geschäftsbedingungen-Richtlinie zugewiesen ist</span><span class="sxs-lookup"><span data-stu-id="9f575-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="9f575-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f575-139">Response</span></span>
<span data-ttu-id="9f575-140">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9f575-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f575-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f575-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f575-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f575-142">Request</span></span>
<span data-ttu-id="9f575-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9f575-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f575-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f575-144">Response</span></span>
<span data-ttu-id="9f575-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f575-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




