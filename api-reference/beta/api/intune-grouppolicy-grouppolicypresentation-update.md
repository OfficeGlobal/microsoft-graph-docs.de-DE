---
title: GroupPolicyPresentation aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentation-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 44da489c3cdf124b434ba35d52d39d63dba54209
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986978"
---
# <a name="update-grouppolicypresentation"></a><span data-ttu-id="1754a-103">GroupPolicyPresentation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1754a-103">Update groupPolicyPresentation</span></span>

> <span data-ttu-id="1754a-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1754a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1754a-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="1754a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1754a-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="1754a-106">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1754a-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="1754a-107">Prerequisites</span></span>
<span data-ttu-id="1754a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1754a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1754a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1754a-110">Permission type</span></span>|<span data-ttu-id="1754a-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1754a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1754a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1754a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1754a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1754a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1754a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1754a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1754a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1754a-115">Not supported.</span></span>|
|<span data-ttu-id="1754a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1754a-116">Application</span></span>|<span data-ttu-id="1754a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1754a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1754a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1754a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="1754a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1754a-119">Request headers</span></span>
|<span data-ttu-id="1754a-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1754a-120">Header</span></span>|<span data-ttu-id="1754a-121">Wert</span><span class="sxs-lookup"><span data-stu-id="1754a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1754a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1754a-122">Authorization</span></span>|<span data-ttu-id="1754a-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="1754a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1754a-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="1754a-124">Accept</span></span>|<span data-ttu-id="1754a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1754a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1754a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1754a-126">Request body</span></span>
<span data-ttu-id="1754a-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="1754a-127">In the request body, supply a JSON representation for the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>

<span data-ttu-id="1754a-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="1754a-128">The following table shows the properties that are required when you create the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md).</span></span>

|<span data-ttu-id="1754a-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1754a-129">Property</span></span>|<span data-ttu-id="1754a-130">Typ</span><span class="sxs-lookup"><span data-stu-id="1754a-130">Type</span></span>|<span data-ttu-id="1754a-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1754a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1754a-132">label</span><span class="sxs-lookup"><span data-stu-id="1754a-132">label</span></span>|<span data-ttu-id="1754a-133">String</span><span class="sxs-lookup"><span data-stu-id="1754a-133">String</span></span>|<span data-ttu-id="1754a-134">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="1754a-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="1754a-135">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="1754a-135">The default value is empty.</span></span>|
|<span data-ttu-id="1754a-136">id</span><span class="sxs-lookup"><span data-stu-id="1754a-136">id</span></span>|<span data-ttu-id="1754a-137">String</span><span class="sxs-lookup"><span data-stu-id="1754a-137">String</span></span>|<span data-ttu-id="1754a-138">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="1754a-138">Key of the entity.</span></span>|
|<span data-ttu-id="1754a-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1754a-139">lastModifiedDateTime</span></span>|<span data-ttu-id="1754a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1754a-140">DateTimeOffset</span></span>|<span data-ttu-id="1754a-141">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="1754a-141">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="1754a-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="1754a-142">Response</span></span>
<span data-ttu-id="1754a-143">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="1754a-143">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1754a-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1754a-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="1754a-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1754a-145">Request</span></span>
<span data-ttu-id="1754a-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1754a-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 92

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="1754a-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="1754a-147">Response</span></span>
<span data-ttu-id="1754a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1754a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 205

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "Label value",
  "id": "a33caa6a-aa6a-a33c-6aaa-3ca36aaa3ca3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




