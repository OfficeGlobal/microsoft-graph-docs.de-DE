---
title: GroupPolicyPresentationListBox aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationListBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 635f78e3bbbde80e0f7107f42d250019198a9887
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961378"
---
# <a name="update-grouppolicypresentationlistbox"></a><span data-ttu-id="28a07-103">GroupPolicyPresentationListBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="28a07-103">Update groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="28a07-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="28a07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28a07-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="28a07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28a07-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="28a07-106">Update the properties of a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28a07-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="28a07-107">Prerequisites</span></span>
<span data-ttu-id="28a07-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28a07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28a07-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="28a07-110">Permission type</span></span>|<span data-ttu-id="28a07-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="28a07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28a07-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="28a07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28a07-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28a07-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="28a07-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="28a07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28a07-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28a07-115">Not supported.</span></span>|
|<span data-ttu-id="28a07-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="28a07-116">Application</span></span>|<span data-ttu-id="28a07-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="28a07-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28a07-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="28a07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="28a07-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="28a07-119">Request headers</span></span>
|<span data-ttu-id="28a07-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="28a07-120">Header</span></span>|<span data-ttu-id="28a07-121">Wert</span><span class="sxs-lookup"><span data-stu-id="28a07-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28a07-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28a07-122">Authorization</span></span>|<span data-ttu-id="28a07-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="28a07-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28a07-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="28a07-124">Accept</span></span>|<span data-ttu-id="28a07-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28a07-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28a07-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="28a07-126">Request body</span></span>
<span data-ttu-id="28a07-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="28a07-127">In the request body, supply a JSON representation for the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

<span data-ttu-id="28a07-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="28a07-128">The following table shows the properties that are required when you create the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span></span>

|<span data-ttu-id="28a07-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="28a07-129">Property</span></span>|<span data-ttu-id="28a07-130">Typ</span><span class="sxs-lookup"><span data-stu-id="28a07-130">Type</span></span>|<span data-ttu-id="28a07-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="28a07-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28a07-132">label</span><span class="sxs-lookup"><span data-stu-id="28a07-132">label</span></span>|<span data-ttu-id="28a07-133">String</span><span class="sxs-lookup"><span data-stu-id="28a07-133">String</span></span>|<span data-ttu-id="28a07-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="28a07-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="28a07-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="28a07-135">The default value is empty.</span></span> <span data-ttu-id="28a07-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="28a07-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="28a07-137">id</span><span class="sxs-lookup"><span data-stu-id="28a07-137">id</span></span>|<span data-ttu-id="28a07-138">String</span><span class="sxs-lookup"><span data-stu-id="28a07-138">String</span></span>|<span data-ttu-id="28a07-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="28a07-139">Key of the entity.</span></span> <span data-ttu-id="28a07-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="28a07-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="28a07-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28a07-141">lastModifiedDateTime</span></span>|<span data-ttu-id="28a07-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28a07-142">DateTimeOffset</span></span>|<span data-ttu-id="28a07-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="28a07-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="28a07-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="28a07-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="28a07-145">explicitValue</span><span class="sxs-lookup"><span data-stu-id="28a07-145">explicitValue</span></span>|<span data-ttu-id="28a07-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="28a07-146">Boolean</span></span>|<span data-ttu-id="28a07-147">Wenn diese Option auf true festgelegt ist, muss der Benutzer den Registrierungsunterschlüssel-Wert und den Registrierungsunterschlüssel Namen angeben.</span><span class="sxs-lookup"><span data-stu-id="28a07-147">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="28a07-148">Das Listenfeld enthält zwei Spalten, eine für den Namen und einen für die Daten.</span><span class="sxs-lookup"><span data-stu-id="28a07-148">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="28a07-149">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="28a07-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="28a07-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="28a07-150">Response</span></span>
<span data-ttu-id="28a07-151">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="28a07-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28a07-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="28a07-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="28a07-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="28a07-153">Request</span></span>
<span data-ttu-id="28a07-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="28a07-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="28a07-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="28a07-155">Response</span></span>
<span data-ttu-id="28a07-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="28a07-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




