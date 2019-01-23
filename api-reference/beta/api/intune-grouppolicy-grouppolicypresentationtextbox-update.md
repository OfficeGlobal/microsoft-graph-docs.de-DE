---
title: GroupPolicyPresentationTextBox aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyPresentationTextBox-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 48417f8d3dcc057e535adcf429cc96922c24162a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431509"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="23a8a-103">GroupPolicyPresentationTextBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="23a8a-103">Update groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="23a8a-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="23a8a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="23a8a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23a8a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23a8a-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="23a8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23a8a-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="23a8a-107">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23a8a-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="23a8a-108">Prerequisites</span></span>
<span data-ttu-id="23a8a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="23a8a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="23a8a-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="23a8a-111">Permission type</span></span>|<span data-ttu-id="23a8a-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="23a8a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23a8a-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="23a8a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23a8a-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23a8a-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="23a8a-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="23a8a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23a8a-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23a8a-116">Not supported.</span></span>|
|<span data-ttu-id="23a8a-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="23a8a-117">Application</span></span>|<span data-ttu-id="23a8a-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="23a8a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23a8a-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="23a8a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="23a8a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="23a8a-120">Request headers</span></span>
|<span data-ttu-id="23a8a-121">Header</span><span class="sxs-lookup"><span data-stu-id="23a8a-121">Header</span></span>|<span data-ttu-id="23a8a-122">Wert</span><span class="sxs-lookup"><span data-stu-id="23a8a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23a8a-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="23a8a-123">Authorization</span></span>|<span data-ttu-id="23a8a-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="23a8a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23a8a-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="23a8a-125">Accept</span></span>|<span data-ttu-id="23a8a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23a8a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23a8a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="23a8a-127">Request body</span></span>
<span data-ttu-id="23a8a-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="23a8a-128">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="23a8a-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="23a8a-129">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="23a8a-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23a8a-130">Property</span></span>|<span data-ttu-id="23a8a-131">Typ</span><span class="sxs-lookup"><span data-stu-id="23a8a-131">Type</span></span>|<span data-ttu-id="23a8a-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23a8a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23a8a-133">label</span><span class="sxs-lookup"><span data-stu-id="23a8a-133">label</span></span>|<span data-ttu-id="23a8a-134">String</span><span class="sxs-lookup"><span data-stu-id="23a8a-134">String</span></span>|<span data-ttu-id="23a8a-135">Lokalisierte Beschriftung für jede Entität Präsentation.</span><span class="sxs-lookup"><span data-stu-id="23a8a-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="23a8a-136">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="23a8a-136">The default value is empty.</span></span> <span data-ttu-id="23a8a-137">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="23a8a-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="23a8a-138">id</span><span class="sxs-lookup"><span data-stu-id="23a8a-138">id</span></span>|<span data-ttu-id="23a8a-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="23a8a-139">String</span></span>|<span data-ttu-id="23a8a-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="23a8a-140">Key of the entity.</span></span> <span data-ttu-id="23a8a-141">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="23a8a-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="23a8a-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23a8a-142">lastModifiedDateTime</span></span>|<span data-ttu-id="23a8a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23a8a-143">DateTimeOffset</span></span>|<span data-ttu-id="23a8a-144">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="23a8a-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="23a8a-145">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="23a8a-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="23a8a-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="23a8a-146">defaultValue</span></span>|<span data-ttu-id="23a8a-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="23a8a-147">String</span></span>|<span data-ttu-id="23a8a-148">Lokalisierte Standardzeichenfolge im Textfeld angezeigt.</span><span class="sxs-lookup"><span data-stu-id="23a8a-148">Localized default string displayed in the text box.</span></span> <span data-ttu-id="23a8a-149">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="23a8a-149">The default value is empty.</span></span>|
|<span data-ttu-id="23a8a-150">erforderlich</span><span class="sxs-lookup"><span data-stu-id="23a8a-150">required</span></span>|<span data-ttu-id="23a8a-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="23a8a-151">Boolean</span></span>|<span data-ttu-id="23a8a-152">Erforderlich, um einen Wert in das Textfeld eingeben.</span><span class="sxs-lookup"><span data-stu-id="23a8a-152">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="23a8a-153">Der Standardwert ist "false".</span><span class="sxs-lookup"><span data-stu-id="23a8a-153">Default value is false.</span></span>|
|<span data-ttu-id="23a8a-154">maxLength</span><span class="sxs-lookup"><span data-stu-id="23a8a-154">maxLength</span></span>|<span data-ttu-id="23a8a-155">Int64</span><span class="sxs-lookup"><span data-stu-id="23a8a-155">Int64</span></span>|<span data-ttu-id="23a8a-156">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Textzeichen angibt.</span><span class="sxs-lookup"><span data-stu-id="23a8a-156">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="23a8a-157">Standardwert ist 1023.</span><span class="sxs-lookup"><span data-stu-id="23a8a-157">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="23a8a-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="23a8a-158">Response</span></span>
<span data-ttu-id="23a8a-159">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="23a8a-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23a8a-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="23a8a-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="23a8a-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="23a8a-161">Request</span></span>
<span data-ttu-id="23a8a-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="23a8a-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
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

### <a name="response"></a><span data-ttu-id="23a8a-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="23a8a-163">Response</span></span>
<span data-ttu-id="23a8a-p109">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="23a8a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




