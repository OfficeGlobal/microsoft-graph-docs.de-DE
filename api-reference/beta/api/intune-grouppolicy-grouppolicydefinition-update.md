---
title: GroupPolicyDefinition aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyDefinition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7b2052d587fc6b5a16ba86b534db9cfca89af3c
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969666"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="421a6-103">GroupPolicyDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="421a6-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="421a6-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="421a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="421a6-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="421a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="421a6-106">Aktualisieren der Eigenschaften eines [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="421a6-106">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="421a6-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="421a6-107">Prerequisites</span></span>
<span data-ttu-id="421a6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="421a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="421a6-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="421a6-110">Permission type</span></span>|<span data-ttu-id="421a6-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="421a6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="421a6-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="421a6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="421a6-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="421a6-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="421a6-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="421a6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="421a6-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="421a6-115">Not supported.</span></span>|
|<span data-ttu-id="421a6-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="421a6-116">Application</span></span>|<span data-ttu-id="421a6-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="421a6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="421a6-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="421a6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="421a6-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="421a6-119">Request headers</span></span>
|<span data-ttu-id="421a6-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="421a6-120">Header</span></span>|<span data-ttu-id="421a6-121">Wert</span><span class="sxs-lookup"><span data-stu-id="421a6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="421a6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="421a6-122">Authorization</span></span>|<span data-ttu-id="421a6-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="421a6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="421a6-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="421a6-124">Accept</span></span>|<span data-ttu-id="421a6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="421a6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="421a6-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="421a6-126">Request body</span></span>
<span data-ttu-id="421a6-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="421a6-127">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="421a6-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="421a6-128">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="421a6-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="421a6-129">Property</span></span>|<span data-ttu-id="421a6-130">Typ</span><span class="sxs-lookup"><span data-stu-id="421a6-130">Type</span></span>|<span data-ttu-id="421a6-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="421a6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="421a6-132">classType</span><span class="sxs-lookup"><span data-stu-id="421a6-132">classType</span></span>|[<span data-ttu-id="421a6-133">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="421a6-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="421a6-134">Gibt den Typ der Gruppen an, auf die die Richtlinie angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="421a6-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="421a6-135">Mögliche Werte sind: `user` und `machine`.</span><span class="sxs-lookup"><span data-stu-id="421a6-135">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="421a6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="421a6-136">displayName</span></span>|<span data-ttu-id="421a6-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="421a6-137">String</span></span>|<span data-ttu-id="421a6-138">Der Name der lokalisierten Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="421a6-138">The localized policy name.</span></span>|
|<span data-ttu-id="421a6-139">explainText</span><span class="sxs-lookup"><span data-stu-id="421a6-139">explainText</span></span>|<span data-ttu-id="421a6-140">String</span><span class="sxs-lookup"><span data-stu-id="421a6-140">String</span></span>|<span data-ttu-id="421a6-141">Die lokalisierte Erläuterung oder der Hilfe Text, der der Richtlinie zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="421a6-141">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="421a6-142">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="421a6-142">The default value is empty.</span></span>|
|<span data-ttu-id="421a6-143">categoryPath</span><span class="sxs-lookup"><span data-stu-id="421a6-143">categoryPath</span></span>|<span data-ttu-id="421a6-144">String</span><span class="sxs-lookup"><span data-stu-id="421a6-144">String</span></span>|<span data-ttu-id="421a6-145">Der lokalisierte vollständige Kategorie-Pfad für die Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="421a6-145">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="421a6-146">supportedOn</span><span class="sxs-lookup"><span data-stu-id="421a6-146">supportedOn</span></span>|<span data-ttu-id="421a6-147">String</span><span class="sxs-lookup"><span data-stu-id="421a6-147">String</span></span>|<span data-ttu-id="421a6-148">Lokalisierte Zeichenfolge, die verwendet wird, um anzugeben, welche Betriebssystem-oder Anwendungsversion von der Richtlinie betroffen ist.</span><span class="sxs-lookup"><span data-stu-id="421a6-148">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="421a6-149">policyType</span><span class="sxs-lookup"><span data-stu-id="421a6-149">policyType</span></span>|[<span data-ttu-id="421a6-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="421a6-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="421a6-151">Gibt den Typ der Gruppenrichtlinie an.</span><span class="sxs-lookup"><span data-stu-id="421a6-151">Specifies the type of group policy.</span></span> <span data-ttu-id="421a6-152">Mögliche Werte: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="421a6-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="421a6-153">id</span><span class="sxs-lookup"><span data-stu-id="421a6-153">id</span></span>|<span data-ttu-id="421a6-154">String</span><span class="sxs-lookup"><span data-stu-id="421a6-154">String</span></span>|<span data-ttu-id="421a6-155">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="421a6-155">Key of the entity.</span></span>|
|<span data-ttu-id="421a6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="421a6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="421a6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="421a6-157">DateTimeOffset</span></span>|<span data-ttu-id="421a6-158">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="421a6-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="421a6-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="421a6-159">Response</span></span>
<span data-ttu-id="421a6-160">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="421a6-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="421a6-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="421a6-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="421a6-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="421a6-162">Request</span></span>
<span data-ttu-id="421a6-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="421a6-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 285

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a><span data-ttu-id="421a6-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="421a6-164">Response</span></span>
<span data-ttu-id="421a6-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="421a6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "id": "f9607947-7947-f960-4779-60f9477960f9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




