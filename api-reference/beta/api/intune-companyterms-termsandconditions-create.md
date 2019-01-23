---
title: Erstellen von „termsAndConditions“
description: Diese Methode erstellt ein neues Objekt des Typs termsAndConditions.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d9bfd5deb96dbfdfac29a16927b4a5289dcfa74a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410350"
---
# <a name="create-termsandconditions"></a><span data-ttu-id="fae05-103">Erstellen von „termsAndConditions“</span><span class="sxs-lookup"><span data-stu-id="fae05-103">Create termsAndConditions</span></span>

> <span data-ttu-id="fae05-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="fae05-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fae05-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fae05-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fae05-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fae05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fae05-107">Diese Methode erstellt ein neues Objekt des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="fae05-107">Create a new [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fae05-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fae05-108">Prerequisites</span></span>
<span data-ttu-id="fae05-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fae05-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fae05-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fae05-111">Permission type</span></span>|<span data-ttu-id="fae05-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fae05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fae05-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fae05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fae05-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fae05-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fae05-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fae05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fae05-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fae05-116">Not supported.</span></span>|
|<span data-ttu-id="fae05-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fae05-117">Application</span></span>|<span data-ttu-id="fae05-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fae05-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fae05-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fae05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="fae05-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fae05-120">Request headers</span></span>
|<span data-ttu-id="fae05-121">Header</span><span class="sxs-lookup"><span data-stu-id="fae05-121">Header</span></span>|<span data-ttu-id="fae05-122">Wert</span><span class="sxs-lookup"><span data-stu-id="fae05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fae05-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="fae05-123">Authorization</span></span>|<span data-ttu-id="fae05-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fae05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fae05-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fae05-125">Accept</span></span>|<span data-ttu-id="fae05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fae05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fae05-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fae05-127">Request body</span></span>
<span data-ttu-id="fae05-128">Geben Sie als Anforderungstext eine JSON-Darstellung des Objekts des Typs „termsAndConditions“ an.</span><span class="sxs-lookup"><span data-stu-id="fae05-128">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="fae05-129">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die angegeben werden müssen, wenn Sie ein Objekt des Typs „termsAndConditions“ erstellen.</span><span class="sxs-lookup"><span data-stu-id="fae05-129">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="fae05-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fae05-130">Property</span></span>|<span data-ttu-id="fae05-131">Typ</span><span class="sxs-lookup"><span data-stu-id="fae05-131">Type</span></span>|<span data-ttu-id="fae05-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fae05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fae05-133">id</span><span class="sxs-lookup"><span data-stu-id="fae05-133">id</span></span>|<span data-ttu-id="fae05-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fae05-134">String</span></span>|<span data-ttu-id="fae05-135">Eindeutiger Bezeichner der Geschäftsbedingungen-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="fae05-135">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="fae05-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fae05-136">createdDateTime</span></span>|<span data-ttu-id="fae05-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fae05-137">DateTimeOffset</span></span>|<span data-ttu-id="fae05-138">Datum und Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fae05-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="fae05-139">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fae05-139">modifiedDateTime</span></span>|<span data-ttu-id="fae05-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fae05-140">DateTimeOffset</span></span>|<span data-ttu-id="fae05-141">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fae05-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="fae05-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fae05-142">lastModifiedDateTime</span></span>|<span data-ttu-id="fae05-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fae05-143">DateTimeOffset</span></span>|<span data-ttu-id="fae05-144">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="fae05-144">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="fae05-145">displayName</span><span class="sxs-lookup"><span data-stu-id="fae05-145">displayName</span></span>|<span data-ttu-id="fae05-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fae05-146">String</span></span>|<span data-ttu-id="fae05-147">Name der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="fae05-147">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="fae05-148">description</span><span class="sxs-lookup"><span data-stu-id="fae05-148">description</span></span>|<span data-ttu-id="fae05-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fae05-149">String</span></span>|<span data-ttu-id="fae05-150">Beschreibung der Geschäftsbedingungen-Richtlinie (vom Administrator festgelegt)</span><span class="sxs-lookup"><span data-stu-id="fae05-150">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="fae05-151">title</span><span class="sxs-lookup"><span data-stu-id="fae05-151">title</span></span>|<span data-ttu-id="fae05-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fae05-152">String</span></span>|<span data-ttu-id="fae05-153">Titel der Geschäftsbedingungen (vom Administrator festgelegt).</span><span class="sxs-lookup"><span data-stu-id="fae05-153">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="fae05-154">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="fae05-154">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="fae05-155">bodyText</span><span class="sxs-lookup"><span data-stu-id="fae05-155">bodyText</span></span>|<span data-ttu-id="fae05-156">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fae05-156">String</span></span>|<span data-ttu-id="fae05-157">Text der Geschäftsbedingungen (vom Administrator festgelegt). In der Regel handelt es sich um die Bedingungen selbst.</span><span class="sxs-lookup"><span data-stu-id="fae05-157">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="fae05-158">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="fae05-158">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="fae05-159">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="fae05-159">acceptanceStatement</span></span>|<span data-ttu-id="fae05-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fae05-160">String</span></span>|<span data-ttu-id="fae05-161">Erläuterung der Geschäftsbedingungen (vom Administrator bereitgestellt). Sie beschreibt in der Regel, was es für den Benutzer bedeutet, wenn er die Geschäftsbedingungen in der Geschäftsbedingungen-Richtlinie annimmt.</span><span class="sxs-lookup"><span data-stu-id="fae05-161">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="fae05-162">Dieser Titel wird Benutzern angezeigt, wenn sie aufgefordert werden, die Geschäftsbedingungen-Richtlinie anzunehmen.</span><span class="sxs-lookup"><span data-stu-id="fae05-162">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="fae05-163">Version</span><span class="sxs-lookup"><span data-stu-id="fae05-163">version</span></span>|<span data-ttu-id="fae05-164">Int32</span><span class="sxs-lookup"><span data-stu-id="fae05-164">Int32</span></span>|<span data-ttu-id="fae05-165">Ganze Zahl, die die aktuelle Version der Geschäftsbedingungen angibt.</span><span class="sxs-lookup"><span data-stu-id="fae05-165">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="fae05-166">Sie wird heraufgesetzt, wenn ein Administrator die Bedingungen ändert und festlegt, dass Benutzer die geänderte Geschäftsbedingungen-Richtlinie erneut annehmen müssen.</span><span class="sxs-lookup"><span data-stu-id="fae05-166">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="fae05-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="fae05-167">Response</span></span>
<span data-ttu-id="fae05-168">Bei erfolgreicher Ausführung gibt die Methode den Antwortcode `201 Created` und ein Objekt des Typs [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fae05-168">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune-companyterms-termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fae05-169">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fae05-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="fae05-170">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fae05-170">Request</span></span>
<span data-ttu-id="fae05-171">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fae05-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions
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

### <a name="response"></a><span data-ttu-id="fae05-172">Antwort</span><span class="sxs-lookup"><span data-stu-id="fae05-172">Response</span></span>
<span data-ttu-id="fae05-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fae05-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




