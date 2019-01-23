---
title: Erstellen von groupPolicyPresentationMultiTextBox
description: Erstellen eines neuen GroupPolicyPresentationMultiTextBox-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41042c5ad62cb56573e924c69b62cef72ee6835c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429927"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="58ceb-103">Erstellen von groupPolicyPresentationMultiTextBox</span><span class="sxs-lookup"><span data-stu-id="58ceb-103">Create groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="58ceb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="58ceb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="58ceb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="58ceb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58ceb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="58ceb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58ceb-107">Erstellen eines neuen [GroupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="58ceb-107">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58ceb-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="58ceb-108">Prerequisites</span></span>
<span data-ttu-id="58ceb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="58ceb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="58ceb-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="58ceb-111">Permission type</span></span>|<span data-ttu-id="58ceb-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="58ceb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58ceb-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="58ceb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58ceb-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58ceb-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="58ceb-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="58ceb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58ceb-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58ceb-116">Not supported.</span></span>|
|<span data-ttu-id="58ceb-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="58ceb-117">Application</span></span>|<span data-ttu-id="58ceb-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="58ceb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58ceb-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="58ceb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="58ceb-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="58ceb-120">Request headers</span></span>
|<span data-ttu-id="58ceb-121">Header</span><span class="sxs-lookup"><span data-stu-id="58ceb-121">Header</span></span>|<span data-ttu-id="58ceb-122">Wert</span><span class="sxs-lookup"><span data-stu-id="58ceb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58ceb-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="58ceb-123">Authorization</span></span>|<span data-ttu-id="58ceb-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="58ceb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58ceb-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="58ceb-125">Accept</span></span>|<span data-ttu-id="58ceb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58ceb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58ceb-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="58ceb-127">Request body</span></span>
<span data-ttu-id="58ceb-128">Geben Sie im Textkörper Anforderung für das Objekt GroupPolicyPresentationMultiTextBox eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="58ceb-128">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="58ceb-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die GroupPolicyPresentationMultiTextBox erstellen.</span><span class="sxs-lookup"><span data-stu-id="58ceb-129">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="58ceb-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="58ceb-130">Property</span></span>|<span data-ttu-id="58ceb-131">Typ</span><span class="sxs-lookup"><span data-stu-id="58ceb-131">Type</span></span>|<span data-ttu-id="58ceb-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="58ceb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58ceb-133">label</span><span class="sxs-lookup"><span data-stu-id="58ceb-133">label</span></span>|<span data-ttu-id="58ceb-134">String</span><span class="sxs-lookup"><span data-stu-id="58ceb-134">String</span></span>|<span data-ttu-id="58ceb-135">Lokalisierte Beschriftung für jede Entität Präsentation.</span><span class="sxs-lookup"><span data-stu-id="58ceb-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="58ceb-136">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="58ceb-136">The default value is empty.</span></span> <span data-ttu-id="58ceb-137">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="58ceb-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="58ceb-138">id</span><span class="sxs-lookup"><span data-stu-id="58ceb-138">id</span></span>|<span data-ttu-id="58ceb-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="58ceb-139">String</span></span>|<span data-ttu-id="58ceb-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="58ceb-140">Key of the entity.</span></span> <span data-ttu-id="58ceb-141">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="58ceb-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="58ceb-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58ceb-142">lastModifiedDateTime</span></span>|<span data-ttu-id="58ceb-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58ceb-143">DateTimeOffset</span></span>|<span data-ttu-id="58ceb-144">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="58ceb-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="58ceb-145">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="58ceb-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="58ceb-146">erforderlich</span><span class="sxs-lookup"><span data-stu-id="58ceb-146">required</span></span>|<span data-ttu-id="58ceb-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="58ceb-147">Boolean</span></span>|<span data-ttu-id="58ceb-148">Erforderlich, um einen Wert in das Textfeld eingeben.</span><span class="sxs-lookup"><span data-stu-id="58ceb-148">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="58ceb-149">Der Standardwert ist "false".</span><span class="sxs-lookup"><span data-stu-id="58ceb-149">Default value is false.</span></span>|
|<span data-ttu-id="58ceb-150">maxLength</span><span class="sxs-lookup"><span data-stu-id="58ceb-150">maxLength</span></span>|<span data-ttu-id="58ceb-151">Int64</span><span class="sxs-lookup"><span data-stu-id="58ceb-151">Int64</span></span>|<span data-ttu-id="58ceb-152">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Textzeichen angibt.</span><span class="sxs-lookup"><span data-stu-id="58ceb-152">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="58ceb-153">Standardwert ist 1023.</span><span class="sxs-lookup"><span data-stu-id="58ceb-153">Default value is 1023.</span></span>|
|<span data-ttu-id="58ceb-154">maxStrings</span><span class="sxs-lookup"><span data-stu-id="58ceb-154">maxStrings</span></span>|<span data-ttu-id="58ceb-155">Int64</span><span class="sxs-lookup"><span data-stu-id="58ceb-155">Int64</span></span>|<span data-ttu-id="58ceb-156">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Zeichenfolgen angibt.</span><span class="sxs-lookup"><span data-stu-id="58ceb-156">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="58ceb-157">Standardwert ist 0.</span><span class="sxs-lookup"><span data-stu-id="58ceb-157">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="58ceb-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="58ceb-158">Response</span></span>
<span data-ttu-id="58ceb-159">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GroupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="58ceb-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58ceb-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="58ceb-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="58ceb-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="58ceb-161">Request</span></span>
<span data-ttu-id="58ceb-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="58ceb-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58ceb-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="58ceb-163">Response</span></span>
<span data-ttu-id="58ceb-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="58ceb-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




