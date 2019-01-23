---
title: Erstellen von groupPolicyPresentationComboBox
description: Erstellen eines neuen GroupPolicyPresentationComboBox-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 328550ed5c07259672ae4debee9a8b28681a4b8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431506"
---
# <a name="create-grouppolicypresentationcombobox"></a><span data-ttu-id="1697f-103">Erstellen von groupPolicyPresentationComboBox</span><span class="sxs-lookup"><span data-stu-id="1697f-103">Create groupPolicyPresentationComboBox</span></span>

> <span data-ttu-id="1697f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1697f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1697f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1697f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1697f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1697f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1697f-107">Erstellen eines neuen [GroupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1697f-107">Create a new [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1697f-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1697f-108">Prerequisites</span></span>
<span data-ttu-id="1697f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1697f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1697f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1697f-111">Permission type</span></span>|<span data-ttu-id="1697f-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1697f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1697f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1697f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1697f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1697f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1697f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1697f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1697f-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1697f-116">Not supported.</span></span>|
|<span data-ttu-id="1697f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1697f-117">Application</span></span>|<span data-ttu-id="1697f-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1697f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1697f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1697f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="1697f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1697f-120">Request headers</span></span>
|<span data-ttu-id="1697f-121">Header</span><span class="sxs-lookup"><span data-stu-id="1697f-121">Header</span></span>|<span data-ttu-id="1697f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1697f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1697f-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="1697f-123">Authorization</span></span>|<span data-ttu-id="1697f-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1697f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1697f-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1697f-125">Accept</span></span>|<span data-ttu-id="1697f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1697f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1697f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1697f-127">Request body</span></span>
<span data-ttu-id="1697f-128">Geben Sie im Textkörper Anforderung für das Objekt GroupPolicyPresentationComboBox eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="1697f-128">In the request body, supply a JSON representation for the groupPolicyPresentationComboBox object.</span></span>

<span data-ttu-id="1697f-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die GroupPolicyPresentationComboBox erstellen.</span><span class="sxs-lookup"><span data-stu-id="1697f-129">The following table shows the properties that are required when you create the groupPolicyPresentationComboBox.</span></span>

|<span data-ttu-id="1697f-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1697f-130">Property</span></span>|<span data-ttu-id="1697f-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1697f-131">Type</span></span>|<span data-ttu-id="1697f-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1697f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1697f-133">label</span><span class="sxs-lookup"><span data-stu-id="1697f-133">label</span></span>|<span data-ttu-id="1697f-134">String</span><span class="sxs-lookup"><span data-stu-id="1697f-134">String</span></span>|<span data-ttu-id="1697f-135">Lokalisierte Beschriftung für jede Entität Präsentation.</span><span class="sxs-lookup"><span data-stu-id="1697f-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="1697f-136">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="1697f-136">The default value is empty.</span></span> <span data-ttu-id="1697f-137">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1697f-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="1697f-138">id</span><span class="sxs-lookup"><span data-stu-id="1697f-138">id</span></span>|<span data-ttu-id="1697f-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1697f-139">String</span></span>|<span data-ttu-id="1697f-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1697f-140">Key of the entity.</span></span> <span data-ttu-id="1697f-141">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1697f-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="1697f-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1697f-142">lastModifiedDateTime</span></span>|<span data-ttu-id="1697f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1697f-143">DateTimeOffset</span></span>|<span data-ttu-id="1697f-144">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="1697f-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="1697f-145">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="1697f-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="1697f-146">defaultValue</span><span class="sxs-lookup"><span data-stu-id="1697f-146">defaultValue</span></span>|<span data-ttu-id="1697f-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1697f-147">String</span></span>|<span data-ttu-id="1697f-148">Lokalisierte Standardzeichenfolge im Kombinationsfeld angezeigt.</span><span class="sxs-lookup"><span data-stu-id="1697f-148">Localized default string displayed in the combo box.</span></span> <span data-ttu-id="1697f-149">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="1697f-149">The default value is empty.</span></span>|
|<span data-ttu-id="1697f-150">Vorschläge</span><span class="sxs-lookup"><span data-stu-id="1697f-150">suggestions</span></span>|<span data-ttu-id="1697f-151">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="1697f-151">String collection</span></span>|<span data-ttu-id="1697f-152">Es werden lokalisierte Zeichenfolgen, die in der Dropdown Liste des Kombinationsfelds aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="1697f-152">Localized strings listed in the drop-down list of the combo box.</span></span> <span data-ttu-id="1697f-153">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="1697f-153">The default value is empty.</span></span>|
|<span data-ttu-id="1697f-154">erforderlich</span><span class="sxs-lookup"><span data-stu-id="1697f-154">required</span></span>|<span data-ttu-id="1697f-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="1697f-155">Boolean</span></span>|<span data-ttu-id="1697f-156">Gibt an, ob ein Wert für den Parameter angegeben werden muss.</span><span class="sxs-lookup"><span data-stu-id="1697f-156">Specifies whether a value must be specified for the parameter.</span></span> <span data-ttu-id="1697f-157">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="1697f-157">The default value is false.</span></span>|
|<span data-ttu-id="1697f-158">maxLength</span><span class="sxs-lookup"><span data-stu-id="1697f-158">maxLength</span></span>|<span data-ttu-id="1697f-159">Int64</span><span class="sxs-lookup"><span data-stu-id="1697f-159">Int64</span></span>|<span data-ttu-id="1697f-160">Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Textzeichen für den Parameter angibt.</span><span class="sxs-lookup"><span data-stu-id="1697f-160">An unsigned integer that specifies the maximum number of text characters for the parameter.</span></span> <span data-ttu-id="1697f-161">Der Standardwert ist 1023.</span><span class="sxs-lookup"><span data-stu-id="1697f-161">The default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="1697f-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="1697f-162">Response</span></span>
<span data-ttu-id="1697f-163">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GroupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1697f-163">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1697f-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1697f-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="1697f-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1697f-165">Request</span></span>
<span data-ttu-id="1697f-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1697f-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="1697f-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="1697f-167">Response</span></span>
<span data-ttu-id="1697f-p110">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1697f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "id": "44332a1d-2a1d-4433-1d2a-33441d2a3344",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```




