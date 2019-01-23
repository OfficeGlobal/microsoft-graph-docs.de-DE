---
title: GroupPolicyPresentationListBox aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyPresentationListBox-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5b443dadcfd913dfd22b2961dea34087ed64a289
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430216"
---
# <a name="update-grouppolicypresentationlistbox"></a><span data-ttu-id="c7753-103">GroupPolicyPresentationListBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="c7753-103">Update groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="c7753-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="c7753-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c7753-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c7753-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7753-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c7753-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7753-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c7753-107">Update the properties of a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7753-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c7753-108">Prerequisites</span></span>
<span data-ttu-id="c7753-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7753-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c7753-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c7753-111">Permission type</span></span>|<span data-ttu-id="c7753-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c7753-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7753-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c7753-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7753-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7753-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c7753-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c7753-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7753-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7753-116">Not supported.</span></span>|
|<span data-ttu-id="c7753-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c7753-117">Application</span></span>|<span data-ttu-id="c7753-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c7753-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7753-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7753-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="c7753-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c7753-120">Request headers</span></span>
|<span data-ttu-id="c7753-121">Header</span><span class="sxs-lookup"><span data-stu-id="c7753-121">Header</span></span>|<span data-ttu-id="c7753-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c7753-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7753-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="c7753-123">Authorization</span></span>|<span data-ttu-id="c7753-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c7753-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7753-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c7753-125">Accept</span></span>|<span data-ttu-id="c7753-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7753-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7753-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c7753-127">Request body</span></span>
<span data-ttu-id="c7753-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="c7753-128">In the request body, supply a JSON representation for the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

<span data-ttu-id="c7753-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="c7753-129">The following table shows the properties that are required when you create the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span></span>

|<span data-ttu-id="c7753-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c7753-130">Property</span></span>|<span data-ttu-id="c7753-131">Typ</span><span class="sxs-lookup"><span data-stu-id="c7753-131">Type</span></span>|<span data-ttu-id="c7753-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c7753-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7753-133">label</span><span class="sxs-lookup"><span data-stu-id="c7753-133">label</span></span>|<span data-ttu-id="c7753-134">String</span><span class="sxs-lookup"><span data-stu-id="c7753-134">String</span></span>|<span data-ttu-id="c7753-135">Lokalisierte Beschriftung für jede Entität Präsentation.</span><span class="sxs-lookup"><span data-stu-id="c7753-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="c7753-136">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="c7753-136">The default value is empty.</span></span> <span data-ttu-id="c7753-137">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c7753-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c7753-138">id</span><span class="sxs-lookup"><span data-stu-id="c7753-138">id</span></span>|<span data-ttu-id="c7753-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c7753-139">String</span></span>|<span data-ttu-id="c7753-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c7753-140">Key of the entity.</span></span> <span data-ttu-id="c7753-141">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c7753-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c7753-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7753-142">lastModifiedDateTime</span></span>|<span data-ttu-id="c7753-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7753-143">DateTimeOffset</span></span>|<span data-ttu-id="c7753-144">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="c7753-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="c7753-145">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="c7753-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="c7753-146">explicitValue</span><span class="sxs-lookup"><span data-stu-id="c7753-146">explicitValue</span></span>|<span data-ttu-id="c7753-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7753-147">Boolean</span></span>|<span data-ttu-id="c7753-148">Wenn diese Option angegeben ist True die Benutzer muss Wert für den Registrierungsunterschlüssel und den Namen des Registrierungs-Unterschlüssels angeben.</span><span class="sxs-lookup"><span data-stu-id="c7753-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="c7753-149">Das Listenfeld enthält zwei Spalten, eine für den Namen und eine für die Daten.</span><span class="sxs-lookup"><span data-stu-id="c7753-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="c7753-150">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="c7753-150">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="c7753-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7753-151">Response</span></span>
<span data-ttu-id="c7753-152">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="c7753-152">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7753-153">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c7753-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7753-154">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c7753-154">Request</span></span>
<span data-ttu-id="c7753-155">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c7753-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true
}
```

### <a name="response"></a><span data-ttu-id="c7753-156">Antwort</span><span class="sxs-lookup"><span data-stu-id="c7753-156">Response</span></span>
<span data-ttu-id="c7753-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c7753-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true
}
```




