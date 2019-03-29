---
title: Aktualisieren von „termsAndConditions“
description: Aktualisiert die Eigenschaften von Objekten des Typs termsAndConditions.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 708d59565896bb7d4782c156dd4af3ff5599b82c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961210"
---
# <a name="update-termsandconditions"></a><span data-ttu-id="1b0d6-103">Aktualisieren von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="1b0d6-103">Update termsAndConditions</span></span>

> <span data-ttu-id="1b0d6-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b0d6-105">Aktualisieren der Eigenschaften eines [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-105">Update the properties of a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b0d6-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1b0d6-106">Prerequisites</span></span>
<span data-ttu-id="1b0d6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b0d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b0d6-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1b0d6-109">Permission type</span></span>|<span data-ttu-id="1b0d6-110">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1b0d6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b0d6-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1b0d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1b0d6-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b0d6-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1b0d6-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1b0d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b0d6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b0d6-114">Not supported.</span></span>|
|<span data-ttu-id="1b0d6-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1b0d6-115">Application</span></span>|<span data-ttu-id="1b0d6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1b0d6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b0d6-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b0d6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="1b0d6-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1b0d6-118">Request headers</span></span>
|<span data-ttu-id="1b0d6-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1b0d6-119">Header</span></span>|<span data-ttu-id="1b0d6-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1b0d6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b0d6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b0d6-121">Authorization</span></span>|<span data-ttu-id="1b0d6-122">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1b0d6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b0d6-123">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1b0d6-123">Accept</span></span>|<span data-ttu-id="1b0d6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1b0d6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b0d6-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1b0d6-125">Request body</span></span>
<span data-ttu-id="1b0d6-126">Geben Sie im Anforderungstext eine JSON-Darstellung des [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-126">In the request body, supply a JSON representation for the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

<span data-ttu-id="1b0d6-127">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-127">The following table shows the properties that are required when you create the [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span></span>

|<span data-ttu-id="1b0d6-128">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1b0d6-128">Property</span></span>|<span data-ttu-id="1b0d6-129">Typ</span><span class="sxs-lookup"><span data-stu-id="1b0d6-129">Type</span></span>|<span data-ttu-id="1b0d6-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1b0d6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b0d6-131">id</span><span class="sxs-lookup"><span data-stu-id="1b0d6-131">id</span></span>|<span data-ttu-id="1b0d6-132">String</span><span class="sxs-lookup"><span data-stu-id="1b0d6-132">String</span></span>|<span data-ttu-id="1b0d6-133">Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="1b0d6-133">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="1b0d6-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0d6-134">createdDateTime</span></span>|<span data-ttu-id="1b0d6-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0d6-135">DateTimeOffset</span></span>|<span data-ttu-id="1b0d6-136">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="1b0d6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0d6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1b0d6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0d6-138">DateTimeOffset</span></span>|<span data-ttu-id="1b0d6-139">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1b0d6-140">displayName</span><span class="sxs-lookup"><span data-stu-id="1b0d6-140">displayName</span></span>|<span data-ttu-id="1b0d6-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b0d6-141">String</span></span>|<span data-ttu-id="1b0d6-142">Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="1b0d6-142">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="1b0d6-143">description</span><span class="sxs-lookup"><span data-stu-id="1b0d6-143">description</span></span>|<span data-ttu-id="1b0d6-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1b0d6-144">String</span></span>|<span data-ttu-id="1b0d6-145">Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="1b0d6-145">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="1b0d6-146">title</span><span class="sxs-lookup"><span data-stu-id="1b0d6-146">title</span></span>|<span data-ttu-id="1b0d6-147">String</span><span class="sxs-lookup"><span data-stu-id="1b0d6-147">String</span></span>|<span data-ttu-id="1b0d6-148">Titel der Geschäftsbedingungen (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="1b0d6-148">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="1b0d6-149">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-149">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="1b0d6-150">bodyText</span><span class="sxs-lookup"><span data-stu-id="1b0d6-150">bodyText</span></span>|<span data-ttu-id="1b0d6-151">String</span><span class="sxs-lookup"><span data-stu-id="1b0d6-151">String</span></span>|<span data-ttu-id="1b0d6-152">Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-152">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="1b0d6-153">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-153">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="1b0d6-154">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="1b0d6-154">acceptanceStatement</span></span>|<span data-ttu-id="1b0d6-155">String</span><span class="sxs-lookup"><span data-stu-id="1b0d6-155">String</span></span>|<span data-ttu-id="1b0d6-156">Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreibt in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-156">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="1b0d6-157">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-157">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="1b0d6-158">Version</span><span class="sxs-lookup"><span data-stu-id="1b0d6-158">version</span></span>|<span data-ttu-id="1b0d6-159">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0d6-159">Int32</span></span>|<span data-ttu-id="1b0d6-160">Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-160">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="1b0d6-161">Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderte Geschäftsbedingungen-Richtlinie erneut annehmen müssen.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-161">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="1b0d6-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b0d6-162">Response</span></span>
<span data-ttu-id="1b0d6-163">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [termsAndConditions](../resources/intune-companyterms-termsandconditions.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-163">If successful, this method returns a `200 OK` response code and an updated [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b0d6-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1b0d6-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b0d6-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1b0d6-165">Request</span></span>
<span data-ttu-id="1b0d6-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}
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

### <a name="response"></a><span data-ttu-id="1b0d6-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="1b0d6-167">Response</span></span>
<span data-ttu-id="1b0d6-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1b0d6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```



