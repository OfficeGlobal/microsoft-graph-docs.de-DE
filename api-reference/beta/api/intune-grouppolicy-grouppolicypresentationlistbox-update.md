---
title: GroupPolicyPresentationListBox aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationListBox-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1eaa079852e90c587f7252d2922a0df5f6ee0ed0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157869"
---
# <a name="update-grouppolicypresentationlistbox"></a><span data-ttu-id="cba3d-103">GroupPolicyPresentationListBox aktualisieren</span><span class="sxs-lookup"><span data-stu-id="cba3d-103">Update groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="cba3d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cba3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cba3d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cba3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cba3d-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="cba3d-106">Update the properties of a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cba3d-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="cba3d-107">Prerequisites</span></span>
<span data-ttu-id="cba3d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cba3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cba3d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cba3d-110">Permission type</span></span>|<span data-ttu-id="cba3d-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cba3d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cba3d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cba3d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cba3d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cba3d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cba3d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cba3d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cba3d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cba3d-115">Not supported.</span></span>|
|<span data-ttu-id="cba3d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cba3d-116">Application</span></span>|<span data-ttu-id="cba3d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cba3d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cba3d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cba3d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="cba3d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cba3d-119">Request headers</span></span>
|<span data-ttu-id="cba3d-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cba3d-120">Header</span></span>|<span data-ttu-id="cba3d-121">Wert</span><span class="sxs-lookup"><span data-stu-id="cba3d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cba3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cba3d-122">Authorization</span></span>|<span data-ttu-id="cba3d-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="cba3d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cba3d-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="cba3d-124">Accept</span></span>|<span data-ttu-id="cba3d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cba3d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cba3d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cba3d-126">Request body</span></span>
<span data-ttu-id="cba3d-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="cba3d-127">In the request body, supply a JSON representation for the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

<span data-ttu-id="cba3d-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="cba3d-128">The following table shows the properties that are required when you create the [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).</span></span>

|<span data-ttu-id="cba3d-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cba3d-129">Property</span></span>|<span data-ttu-id="cba3d-130">Typ</span><span class="sxs-lookup"><span data-stu-id="cba3d-130">Type</span></span>|<span data-ttu-id="cba3d-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cba3d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cba3d-132">label</span><span class="sxs-lookup"><span data-stu-id="cba3d-132">label</span></span>|<span data-ttu-id="cba3d-133">String</span><span class="sxs-lookup"><span data-stu-id="cba3d-133">String</span></span>|<span data-ttu-id="cba3d-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="cba3d-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="cba3d-135">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="cba3d-135">The default value is empty.</span></span> <span data-ttu-id="cba3d-136">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cba3d-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cba3d-137">id</span><span class="sxs-lookup"><span data-stu-id="cba3d-137">id</span></span>|<span data-ttu-id="cba3d-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cba3d-138">String</span></span>|<span data-ttu-id="cba3d-139">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="cba3d-139">Key of the entity.</span></span> <span data-ttu-id="cba3d-140">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cba3d-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cba3d-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cba3d-141">lastModifiedDateTime</span></span>|<span data-ttu-id="cba3d-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cba3d-142">DateTimeOffset</span></span>|<span data-ttu-id="cba3d-143">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="cba3d-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="cba3d-144">Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span><span class="sxs-lookup"><span data-stu-id="cba3d-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="cba3d-145">explicitValue</span><span class="sxs-lookup"><span data-stu-id="cba3d-145">explicitValue</span></span>|<span data-ttu-id="cba3d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="cba3d-146">Boolean</span></span>|<span data-ttu-id="cba3d-147">Wenn diese Option auf true festgelegt ist, muss der Benutzer den Registrierungsunterschlüssel-Wert und den Registrierungsunterschlüssel Namen angeben.</span><span class="sxs-lookup"><span data-stu-id="cba3d-147">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="cba3d-148">Das Listenfeld enthält zwei Spalten, eine für den Namen und einen für die Daten.</span><span class="sxs-lookup"><span data-stu-id="cba3d-148">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="cba3d-149">Der Standardwert ist false.</span><span class="sxs-lookup"><span data-stu-id="cba3d-149">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="cba3d-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="cba3d-150">Response</span></span>
<span data-ttu-id="cba3d-151">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="cba3d-151">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cba3d-152">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cba3d-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="cba3d-153">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cba3d-153">Request</span></span>
<span data-ttu-id="cba3d-154">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cba3d-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cba3d-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="cba3d-155">Response</span></span>
<span data-ttu-id="cba3d-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cba3d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




