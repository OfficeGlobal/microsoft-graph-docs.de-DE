---
title: GroupPolicyPresentationMultiTextBox erstellen
description: Erstellen eines neuen groupPolicyPresentationMultiTextBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bdde2677c4852c70f1693e7a16e2b9e3fb048388
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152101"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="fa94b-103">GroupPolicyPresentationMultiTextBox erstellen</span><span class="sxs-lookup"><span data-stu-id="fa94b-103">Create groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="fa94b-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fa94b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa94b-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fa94b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa94b-106">Erstellen eines neuen [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="fa94b-106">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa94b-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="fa94b-107">Prerequisites</span></span>
<span data-ttu-id="fa94b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fa94b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fa94b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fa94b-110">Permission type</span></span>|<span data-ttu-id="fa94b-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fa94b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa94b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fa94b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa94b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa94b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fa94b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fa94b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa94b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa94b-115">Not supported.</span></span>|
|<span data-ttu-id="fa94b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fa94b-116">Application</span></span>|<span data-ttu-id="fa94b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fa94b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa94b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa94b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="fa94b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fa94b-119">Request headers</span></span>
|<span data-ttu-id="fa94b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="fa94b-120">Header</span></span>|<span data-ttu-id="fa94b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="fa94b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa94b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa94b-122">Authorization</span></span>|<span data-ttu-id="fa94b-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa94b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa94b-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="fa94b-124">Accept</span></span>|<span data-ttu-id="fa94b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa94b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa94b-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fa94b-126">Request body</span></span>
<span data-ttu-id="fa94b-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationMultiTextBox-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="fa94b-127">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="fa94b-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationMultiTextBox erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fa94b-128">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="fa94b-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fa94b-129">Property</span></span>|<span data-ttu-id="fa94b-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fa94b-130">Type</span></span>|<span data-ttu-id="fa94b-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fa94b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa94b-132">label</span><span class="sxs-lookup"><span data-stu-id="fa94b-132">label</span></span>|<span data-ttu-id="fa94b-133">String</span><span class="sxs-lookup"><span data-stu-id="fa94b-133">String</span></span>|<span data-ttu-id="fa94b-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="fa94b-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="fa94b-135">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="fa94b-135">The default value is empty.</span></span> <span data-ttu-id="fa94b-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fa94b-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="fa94b-137">id</span><span class="sxs-lookup"><span data-stu-id="fa94b-137">id</span></span>|<span data-ttu-id="fa94b-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fa94b-138">String</span></span>|<span data-ttu-id="fa94b-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="fa94b-139">Key of the entity.</span></span> <span data-ttu-id="fa94b-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fa94b-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="fa94b-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa94b-141">lastModifiedDateTime</span></span>|<span data-ttu-id="fa94b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa94b-142">DateTimeOffset</span></span>|<span data-ttu-id="fa94b-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="fa94b-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="fa94b-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="fa94b-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="fa94b-145">erforderlich</span><span class="sxs-lookup"><span data-stu-id="fa94b-145">required</span></span>|<span data-ttu-id="fa94b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa94b-146">Boolean</span></span>|<span data-ttu-id="fa94b-147">Anforderung zur Eingabe eines Werts in das Textfeld.</span><span class="sxs-lookup"><span data-stu-id="fa94b-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="fa94b-148">Der Standardwert ist "false".</span><span class="sxs-lookup"><span data-stu-id="fa94b-148">Default value is false.</span></span>|
|<span data-ttu-id="fa94b-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="fa94b-149">maxLength</span></span>|<span data-ttu-id="fa94b-150">Int64</span><span class="sxs-lookup"><span data-stu-id="fa94b-150">Int64</span></span>|<span data-ttu-id="fa94b-151">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Textzeichen angibt.</span><span class="sxs-lookup"><span data-stu-id="fa94b-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="fa94b-152">Der Standardwert ist 1023.</span><span class="sxs-lookup"><span data-stu-id="fa94b-152">Default value is 1023.</span></span>|
|<span data-ttu-id="fa94b-153">maxStrings</span><span class="sxs-lookup"><span data-stu-id="fa94b-153">maxStrings</span></span>|<span data-ttu-id="fa94b-154">Int64</span><span class="sxs-lookup"><span data-stu-id="fa94b-154">Int64</span></span>|<span data-ttu-id="fa94b-155">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Zeichenfolgen angibt.</span><span class="sxs-lookup"><span data-stu-id="fa94b-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="fa94b-156">Der Standardwert ist 0.</span><span class="sxs-lookup"><span data-stu-id="fa94b-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="fa94b-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa94b-157">Response</span></span>
<span data-ttu-id="fa94b-158">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="fa94b-158">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa94b-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fa94b-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa94b-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fa94b-160">Request</span></span>
<span data-ttu-id="fa94b-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fa94b-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```

### <a name="response"></a><span data-ttu-id="fa94b-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="fa94b-162">Response</span></span>
<span data-ttu-id="fa94b-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fa94b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "id": "381ac035-c035-381a-35c0-1a3835c01a38",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```




