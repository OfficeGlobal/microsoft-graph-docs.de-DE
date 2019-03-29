---
title: GroupPolicyPresentationTextBox erstellen
description: Erstellen eines neuen groupPolicyPresentationTextBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6c2800f1fecd6c1d7355aa482125505cda19694
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975987"
---
# <a name="create-grouppolicypresentationtextbox"></a><span data-ttu-id="0f9c6-103">GroupPolicyPresentationTextBox erstellen</span><span class="sxs-lookup"><span data-stu-id="0f9c6-103">Create groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="0f9c6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f9c6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f9c6-106">Erstellen eines neuen [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-106">Create a new [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f9c6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0f9c6-107">Prerequisites</span></span>
<span data-ttu-id="0f9c6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f9c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f9c6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0f9c6-110">Permission type</span></span>|<span data-ttu-id="0f9c6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0f9c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f9c6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0f9c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f9c6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f9c6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0f9c6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0f9c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f9c6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f9c6-115">Not supported.</span></span>|
|<span data-ttu-id="0f9c6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0f9c6-116">Application</span></span>|<span data-ttu-id="0f9c6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0f9c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f9c6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f9c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="0f9c6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0f9c6-119">Request headers</span></span>
|<span data-ttu-id="0f9c6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0f9c6-120">Header</span></span>|<span data-ttu-id="0f9c6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0f9c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f9c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f9c6-122">Authorization</span></span>|<span data-ttu-id="0f9c6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0f9c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f9c6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0f9c6-124">Accept</span></span>|<span data-ttu-id="0f9c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f9c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f9c6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0f9c6-126">Request body</span></span>
<span data-ttu-id="0f9c6-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyPresentationTextBox-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-127">In the request body, supply a JSON representation for the groupPolicyPresentationTextBox object.</span></span>

<span data-ttu-id="0f9c6-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyPresentationTextBox erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-128">The following table shows the properties that are required when you create the groupPolicyPresentationTextBox.</span></span>

|<span data-ttu-id="0f9c6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0f9c6-129">Property</span></span>|<span data-ttu-id="0f9c6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0f9c6-130">Type</span></span>|<span data-ttu-id="0f9c6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0f9c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f9c6-132">label</span><span class="sxs-lookup"><span data-stu-id="0f9c6-132">label</span></span>|<span data-ttu-id="0f9c6-133">String</span><span class="sxs-lookup"><span data-stu-id="0f9c6-133">String</span></span>|<span data-ttu-id="0f9c6-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="0f9c6-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-135">The default value is empty.</span></span> <span data-ttu-id="0f9c6-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="0f9c6-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0f9c6-137">id</span><span class="sxs-lookup"><span data-stu-id="0f9c6-137">id</span></span>|<span data-ttu-id="0f9c6-138">String</span><span class="sxs-lookup"><span data-stu-id="0f9c6-138">String</span></span>|<span data-ttu-id="0f9c6-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0f9c6-139">Key of the entity.</span></span> <span data-ttu-id="0f9c6-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="0f9c6-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0f9c6-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f9c6-141">lastModifiedDateTime</span></span>|<span data-ttu-id="0f9c6-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f9c6-142">DateTimeOffset</span></span>|<span data-ttu-id="0f9c6-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="0f9c6-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="0f9c6-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="0f9c6-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="0f9c6-145">defaultValue</span></span>|<span data-ttu-id="0f9c6-146">String</span><span class="sxs-lookup"><span data-stu-id="0f9c6-146">String</span></span>|<span data-ttu-id="0f9c6-147">Lokalisierte Standardzeichenfolge, die im Textfeld angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-147">Localized default string displayed in the text box.</span></span> <span data-ttu-id="0f9c6-148">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-148">The default value is empty.</span></span>|
|<span data-ttu-id="0f9c6-149">erforderlich</span><span class="sxs-lookup"><span data-stu-id="0f9c6-149">required</span></span>|<span data-ttu-id="0f9c6-150">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0f9c6-150">Boolean</span></span>|<span data-ttu-id="0f9c6-151">Anforderung zur Eingabe eines Werts in das Textfeld.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-151">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="0f9c6-152">Standardwert ist "false".</span><span class="sxs-lookup"><span data-stu-id="0f9c6-152">Default value is false.</span></span>|
|<span data-ttu-id="0f9c6-153">maxLength</span><span class="sxs-lookup"><span data-stu-id="0f9c6-153">maxLength</span></span>|<span data-ttu-id="0f9c6-154">Int64</span><span class="sxs-lookup"><span data-stu-id="0f9c6-154">Int64</span></span>|<span data-ttu-id="0f9c6-155">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Textzeichen angibt.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-155">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="0f9c6-156">Der Standardwert ist 1023.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-156">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="0f9c6-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f9c6-157">Response</span></span>
<span data-ttu-id="0f9c6-158">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-158">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f9c6-159">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0f9c6-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f9c6-160">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0f9c6-160">Request</span></span>
<span data-ttu-id="0f9c6-161">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="0f9c6-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="0f9c6-162">Response</span></span>
<span data-ttu-id="0f9c6-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0f9c6-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```




