---
title: Erstellen von „termsAndConditions“
description: Diese Methode erstellt ein neues Objekt des Typs termsAndConditions.
ms.openlocfilehash: 1947a41ddfe108d8f44c899786d0b0b129ac6939
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064288"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="9d9a0-103">Erstellen von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="9d9a0-103">Create termsAndConditions</span></span>

> <span data-ttu-id="9d9a0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d9a0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d9a0-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d9a0-107">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="9d9a0-107">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d9a0-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="9d9a0-108">Prerequisites</span></span>
<span data-ttu-id="9d9a0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d9a0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d9a0-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9d9a0-111">Permission type</span></span>|<span data-ttu-id="9d9a0-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9d9a0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d9a0-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9d9a0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d9a0-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d9a0-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9d9a0-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9d9a0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d9a0-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d9a0-116">Not supported.</span></span>|
|<span data-ttu-id="9d9a0-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9d9a0-117">Application</span></span>|<span data-ttu-id="9d9a0-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9d9a0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d9a0-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d9a0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="9d9a0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9d9a0-120">Request headers</span></span>
|<span data-ttu-id="9d9a0-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9d9a0-121">Header</span></span>|<span data-ttu-id="9d9a0-122">Wert</span><span class="sxs-lookup"><span data-stu-id="9d9a0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d9a0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d9a0-123">Authorization</span></span>|<span data-ttu-id="9d9a0-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="9d9a0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d9a0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d9a0-125">Accept</span></span>|<span data-ttu-id="9d9a0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d9a0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d9a0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9d9a0-127">Request body</span></span>
<span data-ttu-id="9d9a0-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditions“ an.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-128">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="9d9a0-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditions“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-129">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="9d9a0-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9d9a0-130">Property</span></span>|<span data-ttu-id="9d9a0-131">Typ</span><span class="sxs-lookup"><span data-stu-id="9d9a0-131">Type</span></span>|<span data-ttu-id="9d9a0-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9d9a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d9a0-133">id</span><span class="sxs-lookup"><span data-stu-id="9d9a0-133">id</span></span>|<span data-ttu-id="9d9a0-134">String</span><span class="sxs-lookup"><span data-stu-id="9d9a0-134">String</span></span>|<span data-ttu-id="9d9a0-135">Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="9d9a0-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="9d9a0-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d9a0-136">createdDateTime</span></span>|<span data-ttu-id="9d9a0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d9a0-137">DateTimeOffset</span></span>|<span data-ttu-id="9d9a0-138">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="9d9a0-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d9a0-139">modifiedDateTime</span></span>|<span data-ttu-id="9d9a0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d9a0-140">DateTimeOffset</span></span>|<span data-ttu-id="9d9a0-141">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9d9a0-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d9a0-142">lastModifiedDateTime</span></span>|<span data-ttu-id="9d9a0-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d9a0-143">DateTimeOffset</span></span>|<span data-ttu-id="9d9a0-144">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="9d9a0-145">displayName</span><span class="sxs-lookup"><span data-stu-id="9d9a0-145">displayName</span></span>|<span data-ttu-id="9d9a0-146">String</span><span class="sxs-lookup"><span data-stu-id="9d9a0-146">String</span></span>|<span data-ttu-id="9d9a0-147">Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="9d9a0-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="9d9a0-148">description</span><span class="sxs-lookup"><span data-stu-id="9d9a0-148">description</span></span>|<span data-ttu-id="9d9a0-149">String</span><span class="sxs-lookup"><span data-stu-id="9d9a0-149">String</span></span>|<span data-ttu-id="9d9a0-150">Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="9d9a0-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="9d9a0-151">title</span><span class="sxs-lookup"><span data-stu-id="9d9a0-151">title</span></span>|<span data-ttu-id="9d9a0-152">String</span><span class="sxs-lookup"><span data-stu-id="9d9a0-152">String</span></span>|<span data-ttu-id="9d9a0-153">Titel der Geschäftsbedingungen (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="9d9a0-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="9d9a0-154">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="9d9a0-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="9d9a0-155">bodyText</span></span>|<span data-ttu-id="9d9a0-156">String</span><span class="sxs-lookup"><span data-stu-id="9d9a0-156">String</span></span>|<span data-ttu-id="9d9a0-157">Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="9d9a0-158">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="9d9a0-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="9d9a0-159">acceptanceStatement</span></span>|<span data-ttu-id="9d9a0-160">String</span><span class="sxs-lookup"><span data-stu-id="9d9a0-160">String</span></span>|<span data-ttu-id="9d9a0-161">Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreibt in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="9d9a0-162">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="9d9a0-163">Version</span><span class="sxs-lookup"><span data-stu-id="9d9a0-163">version</span></span>|<span data-ttu-id="9d9a0-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9d9a0-164">Int32</span></span>|<span data-ttu-id="9d9a0-165">Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="9d9a0-166">Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderte Geschäftsbedingungen-Richtlinie erneut annehmen müssen.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="9d9a0-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d9a0-167">Response</span></span>
<span data-ttu-id="9d9a0-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-168">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d9a0-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9d9a0-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d9a0-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9d9a0-170">Request</span></span>
<span data-ttu-id="9d9a0-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 337

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="9d9a0-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="9d9a0-172">Response</span></span>
<span data-ttu-id="9d9a0-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9d9a0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





