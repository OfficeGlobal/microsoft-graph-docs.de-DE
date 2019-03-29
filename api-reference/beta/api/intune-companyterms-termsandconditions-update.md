---
title: Aktualisieren von „termsAndConditions“
description: Aktualisiert die Eigenschaften von Objekten des Typs termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1855a5b3c4933b7304b9b984ab96aaaaab0b675
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957416"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="15436-103">Aktualisieren von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="15436-103">Update termsAndConditions</span></span>

> <span data-ttu-id="15436-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15436-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15436-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="15436-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15436-106">Aktualisieren der Eigenschaften eines [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="15436-106">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15436-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="15436-107">Prerequisites</span></span>
<span data-ttu-id="15436-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15436-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15436-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="15436-110">Permission type</span></span>|<span data-ttu-id="15436-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="15436-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15436-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="15436-112">Delegated (work or school account)</span></span>|<span data-ttu-id="15436-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15436-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="15436-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="15436-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15436-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15436-115">Not supported.</span></span>|
|<span data-ttu-id="15436-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="15436-116">Application</span></span>|<span data-ttu-id="15436-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="15436-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="15436-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="15436-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments/{termsAndConditionsGroupAssignmentId}/termsAndConditions
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="15436-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="15436-119">Request headers</span></span>
|<span data-ttu-id="15436-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="15436-120">Header</span></span>|<span data-ttu-id="15436-121">Wert</span><span class="sxs-lookup"><span data-stu-id="15436-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15436-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15436-122">Authorization</span></span>|<span data-ttu-id="15436-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="15436-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15436-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="15436-124">Accept</span></span>|<span data-ttu-id="15436-125">application/json</span><span class="sxs-lookup"><span data-stu-id="15436-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15436-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="15436-126">Request body</span></span>
<span data-ttu-id="15436-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="15436-127">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="15436-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="15436-128">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="15436-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15436-129">Property</span></span>|<span data-ttu-id="15436-130">Typ</span><span class="sxs-lookup"><span data-stu-id="15436-130">Type</span></span>|<span data-ttu-id="15436-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15436-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15436-132">id</span><span class="sxs-lookup"><span data-stu-id="15436-132">id</span></span>|<span data-ttu-id="15436-133">String</span><span class="sxs-lookup"><span data-stu-id="15436-133">String</span></span>|<span data-ttu-id="15436-134">Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="15436-134">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="15436-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15436-135">createdDateTime</span></span>|<span data-ttu-id="15436-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15436-136">DateTimeOffset</span></span>|<span data-ttu-id="15436-137">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="15436-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="15436-138">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15436-138">modifiedDateTime</span></span>|<span data-ttu-id="15436-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15436-139">DateTimeOffset</span></span>|<span data-ttu-id="15436-140">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="15436-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="15436-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15436-141">lastModifiedDateTime</span></span>|<span data-ttu-id="15436-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15436-142">DateTimeOffset</span></span>|<span data-ttu-id="15436-143">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="15436-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="15436-144">displayName</span><span class="sxs-lookup"><span data-stu-id="15436-144">displayName</span></span>|<span data-ttu-id="15436-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15436-145">String</span></span>|<span data-ttu-id="15436-146">Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="15436-146">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="15436-147">description</span><span class="sxs-lookup"><span data-stu-id="15436-147">description</span></span>|<span data-ttu-id="15436-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="15436-148">String</span></span>|<span data-ttu-id="15436-149">Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="15436-149">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="15436-150">title</span><span class="sxs-lookup"><span data-stu-id="15436-150">title</span></span>|<span data-ttu-id="15436-151">String</span><span class="sxs-lookup"><span data-stu-id="15436-151">String</span></span>|<span data-ttu-id="15436-152">Titel der Geschäftsbedingungen (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="15436-152">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="15436-153">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="15436-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="15436-154">bodyText</span><span class="sxs-lookup"><span data-stu-id="15436-154">bodyText</span></span>|<span data-ttu-id="15436-155">String</span><span class="sxs-lookup"><span data-stu-id="15436-155">String</span></span>|<span data-ttu-id="15436-156">Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst.</span><span class="sxs-lookup"><span data-stu-id="15436-156">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="15436-157">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="15436-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="15436-158">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="15436-158">acceptanceStatement</span></span>|<span data-ttu-id="15436-159">String</span><span class="sxs-lookup"><span data-stu-id="15436-159">String</span></span>|<span data-ttu-id="15436-160">Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreibt in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt.</span><span class="sxs-lookup"><span data-stu-id="15436-160">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="15436-161">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="15436-161">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="15436-162">Version</span><span class="sxs-lookup"><span data-stu-id="15436-162">version</span></span>|<span data-ttu-id="15436-163">Int32</span><span class="sxs-lookup"><span data-stu-id="15436-163">Int32</span></span>|<span data-ttu-id="15436-164">Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt.</span><span class="sxs-lookup"><span data-stu-id="15436-164">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="15436-165">Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderte Geschäftsbedingungen-Richtlinie erneut annehmen müssen.</span><span class="sxs-lookup"><span data-stu-id="15436-165">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="15436-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="15436-166">Response</span></span>
<span data-ttu-id="15436-167">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15436-167">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15436-168">Beispiel</span><span class="sxs-lookup"><span data-stu-id="15436-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="15436-169">Anforderung</span><span class="sxs-lookup"><span data-stu-id="15436-169">Request</span></span>
<span data-ttu-id="15436-170">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="15436-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="15436-171">Antwort</span><span class="sxs-lookup"><span data-stu-id="15436-171">Response</span></span>
<span data-ttu-id="15436-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="15436-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 505

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```




