---
title: GroupPolicyDefinition aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyDefinition-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eeb3e32f1870eac8491989426081df2ae41e4d42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429991"
---
# <a name="update-grouppolicydefinition"></a><span data-ttu-id="948f1-103">GroupPolicyDefinition aktualisieren</span><span class="sxs-lookup"><span data-stu-id="948f1-103">Update groupPolicyDefinition</span></span>

> <span data-ttu-id="948f1-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="948f1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="948f1-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="948f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="948f1-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="948f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="948f1-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="948f1-107">Update the properties of a [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="948f1-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="948f1-108">Prerequisites</span></span>
<span data-ttu-id="948f1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="948f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="948f1-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="948f1-111">Permission type</span></span>|<span data-ttu-id="948f1-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="948f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="948f1-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="948f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="948f1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="948f1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="948f1-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="948f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="948f1-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="948f1-116">Not supported.</span></span>|
|<span data-ttu-id="948f1-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="948f1-117">Application</span></span>|<span data-ttu-id="948f1-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="948f1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="948f1-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="948f1-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="948f1-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="948f1-120">Request headers</span></span>
|<span data-ttu-id="948f1-121">Header</span><span class="sxs-lookup"><span data-stu-id="948f1-121">Header</span></span>|<span data-ttu-id="948f1-122">Wert</span><span class="sxs-lookup"><span data-stu-id="948f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="948f1-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="948f1-123">Authorization</span></span>|<span data-ttu-id="948f1-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="948f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="948f1-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="948f1-125">Accept</span></span>|<span data-ttu-id="948f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="948f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="948f1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="948f1-127">Request body</span></span>
<span data-ttu-id="948f1-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="948f1-128">In the request body, supply a JSON representation for the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object.</span></span>

<span data-ttu-id="948f1-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="948f1-129">The following table shows the properties that are required when you create the [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md).</span></span>

|<span data-ttu-id="948f1-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="948f1-130">Property</span></span>|<span data-ttu-id="948f1-131">Typ</span><span class="sxs-lookup"><span data-stu-id="948f1-131">Type</span></span>|<span data-ttu-id="948f1-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="948f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="948f1-133">classType</span><span class="sxs-lookup"><span data-stu-id="948f1-133">classType</span></span>|[<span data-ttu-id="948f1-134">groupPolicyDefinitionClassType</span><span class="sxs-lookup"><span data-stu-id="948f1-134">groupPolicyDefinitionClassType</span></span>](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|<span data-ttu-id="948f1-135">Identifiziert den Typ von Gruppen, denen auf die Richtlinie angewendet werden kann.</span><span class="sxs-lookup"><span data-stu-id="948f1-135">Identifies the type of groups the policy can be applied to.</span></span> <span data-ttu-id="948f1-136">Mögliche Werte sind: `user`, `machine` und `both`.</span><span class="sxs-lookup"><span data-stu-id="948f1-136">Possible values are: `user`, `machine`, `both`.</span></span>|
|<span data-ttu-id="948f1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="948f1-137">displayName</span></span>|<span data-ttu-id="948f1-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="948f1-138">String</span></span>|<span data-ttu-id="948f1-139">Die lokalisierten Richtliniennamen.</span><span class="sxs-lookup"><span data-stu-id="948f1-139">The localized policy name.</span></span>|
|<span data-ttu-id="948f1-140">explainText</span><span class="sxs-lookup"><span data-stu-id="948f1-140">explainText</span></span>|<span data-ttu-id="948f1-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="948f1-141">String</span></span>|<span data-ttu-id="948f1-142">Die lokalisierten Erläuterung oder Hilfe Text mit der Richtlinie verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="948f1-142">The localized explanation or help text associated with the policy.</span></span> <span data-ttu-id="948f1-143">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="948f1-143">The default value is empty.</span></span>|
|<span data-ttu-id="948f1-144">categoryPath</span><span class="sxs-lookup"><span data-stu-id="948f1-144">categoryPath</span></span>|<span data-ttu-id="948f1-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="948f1-145">String</span></span>|<span data-ttu-id="948f1-146">Der Pfad der lokalisierte vollständige Kategorie für die Richtlinie ein.</span><span class="sxs-lookup"><span data-stu-id="948f1-146">The localized full category path for the policy.</span></span>|
|<span data-ttu-id="948f1-147">supportedOn</span><span class="sxs-lookup"><span data-stu-id="948f1-147">supportedOn</span></span>|<span data-ttu-id="948f1-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="948f1-148">String</span></span>|<span data-ttu-id="948f1-149">Lokalisierte Zeichenfolge verwendet, um anzugeben, welche Version der Anwendung oder das Betriebssystem durch die Richtlinie betroffen ist.</span><span class="sxs-lookup"><span data-stu-id="948f1-149">Localized string used to specify what operating system or application version is affected by the policy.</span></span>|
|<span data-ttu-id="948f1-150">policyType</span><span class="sxs-lookup"><span data-stu-id="948f1-150">policyType</span></span>|[<span data-ttu-id="948f1-151">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="948f1-151">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="948f1-152">Gibt den Typ von Gruppenrichtlinien.</span><span class="sxs-lookup"><span data-stu-id="948f1-152">Specifies the type of group policy.</span></span> <span data-ttu-id="948f1-153">Mögliche Werte sind: `admxBacked` und `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="948f1-153">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="948f1-154">id</span><span class="sxs-lookup"><span data-stu-id="948f1-154">id</span></span>|<span data-ttu-id="948f1-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="948f1-155">String</span></span>|<span data-ttu-id="948f1-156">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="948f1-156">Key of the entity.</span></span>|
|<span data-ttu-id="948f1-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="948f1-157">lastModifiedDateTime</span></span>|<span data-ttu-id="948f1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="948f1-158">DateTimeOffset</span></span>|<span data-ttu-id="948f1-159">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="948f1-159">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="948f1-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="948f1-160">Response</span></span>
<span data-ttu-id="948f1-161">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="948f1-161">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="948f1-162">Beispiel</span><span class="sxs-lookup"><span data-stu-id="948f1-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="948f1-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="948f1-163">Request</span></span>
<span data-ttu-id="948f1-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="948f1-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="948f1-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="948f1-165">Response</span></span>
<span data-ttu-id="948f1-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="948f1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




