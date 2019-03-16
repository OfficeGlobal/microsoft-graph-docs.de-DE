---
title: GroupPolicyDefinition aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyDefinition-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f750e7f6a3bd631973fdeabc59011d0d07301cb4
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644293"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="750bc-103">GroupPolicyDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="750bc-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="750bc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="750bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="750bc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="750bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="750bc-106">Aktualisieren der Eigenschaften eines [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="750bc-106">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="750bc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="750bc-107">Prerequisites</span></span>
<span data-ttu-id="750bc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="750bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="750bc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="750bc-110">Permission type</span></span>|<span data-ttu-id="750bc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="750bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="750bc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="750bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="750bc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="750bc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="750bc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="750bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="750bc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="750bc-115">Not supported.</span></span>|
|<span data-ttu-id="750bc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="750bc-116">Application</span></span>|<span data-ttu-id="750bc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="750bc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="750bc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="750bc-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="750bc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="750bc-119">Request headers</span></span>
|<span data-ttu-id="750bc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="750bc-120">Header</span></span>|<span data-ttu-id="750bc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="750bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="750bc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="750bc-122">Authorization</span></span>|<span data-ttu-id="750bc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="750bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="750bc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="750bc-124">Accept</span></span>|<span data-ttu-id="750bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="750bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="750bc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="750bc-126">Request body</span></span>
<span data-ttu-id="750bc-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="750bc-127">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="750bc-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="750bc-128">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="750bc-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="750bc-129">Property</span></span>|<span data-ttu-id="750bc-130">Typ</span><span class="sxs-lookup"><span data-stu-id="750bc-130">Type</span></span>|<span data-ttu-id="750bc-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="750bc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="750bc-132">classType</span><span class="sxs-lookup"><span data-stu-id="750bc-132">classType</span></span>|[<span data-ttu-id="750bc-133">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="750bc-133">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="750bc-134">Gibt den Typ der Gruppen an, auf die die Richtlinie angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="750bc-134">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="750bc-135">Mögliche Werte sind: `user` und `machine`.</span><span class="sxs-lookup"><span data-stu-id="750bc-135">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="750bc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="750bc-136">displayName</span></span>|<span data-ttu-id="750bc-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="750bc-137">String</span></span>|<span data-ttu-id="750bc-138">Der Name der lokalisierten Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="750bc-138">The localized policy name.</span></span>|
|<span data-ttu-id="750bc-139">explainText</span><span class="sxs-lookup"><span data-stu-id="750bc-139">explainText</span></span>|<span data-ttu-id="750bc-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="750bc-140">String</span></span>|<span data-ttu-id="750bc-141">Die lokalisierte Erläuterung oder der Hilfe Text, der der Richtlinie zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="750bc-141">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="750bc-142">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="750bc-142">The default value is empty.</span></span>|
|<span data-ttu-id="750bc-143">categoryPath</span><span class="sxs-lookup"><span data-stu-id="750bc-143">categoryPath</span></span>|<span data-ttu-id="750bc-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="750bc-144">String</span></span>|<span data-ttu-id="750bc-145">Der lokalisierte vollständige Kategorie-Pfad für die Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="750bc-145">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="750bc-146">supportedOn</span><span class="sxs-lookup"><span data-stu-id="750bc-146">supportedOn</span></span>|<span data-ttu-id="750bc-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="750bc-147">String</span></span>|<span data-ttu-id="750bc-148">Lokalisierte Zeichenfolge, die verwendet wird, um anzugeben, welche Betriebssystem-oder Anwendungsversion von der Richtlinie betroffen ist.</span><span class="sxs-lookup"><span data-stu-id="750bc-148">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="750bc-149">policyType</span><span class="sxs-lookup"><span data-stu-id="750bc-149">policyType</span></span>|[<span data-ttu-id="750bc-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="750bc-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="750bc-151">Gibt den Typ der Gruppenrichtlinie an.</span><span class="sxs-lookup"><span data-stu-id="750bc-151">Specifies the type of group policy.</span></span> <span data-ttu-id="750bc-152">Mögliche Werte: `admxBacked`, `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="750bc-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="750bc-153">id</span><span class="sxs-lookup"><span data-stu-id="750bc-153">id</span></span>|<span data-ttu-id="750bc-154">String</span><span class="sxs-lookup"><span data-stu-id="750bc-154">String</span></span>|<span data-ttu-id="750bc-155">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="750bc-155">Key of the entity.</span></span>|
|<span data-ttu-id="750bc-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="750bc-156">lastModifiedDateTime</span></span>|<span data-ttu-id="750bc-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="750bc-157">DateTimeOffset</span></span>|<span data-ttu-id="750bc-158">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="750bc-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="750bc-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="750bc-159">Response</span></span>
<span data-ttu-id="750bc-160">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="750bc-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="750bc-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="750bc-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="750bc-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="750bc-162">Request</span></span>
<span data-ttu-id="750bc-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="750bc-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="750bc-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="750bc-164">Response</span></span>
<span data-ttu-id="750bc-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="750bc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




