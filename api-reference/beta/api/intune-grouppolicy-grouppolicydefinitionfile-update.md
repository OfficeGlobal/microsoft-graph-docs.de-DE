---
title: GroupPolicyDefinitionFile aktualisieren
description: Aktualisieren Sie die Eigenschaften eines GroupPolicyDefinitionFile-Objekts.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be713dba2d503f19cd565fe5e53d252ed20667e0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430143"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="bc31d-103">GroupPolicyDefinitionFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bc31d-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="bc31d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="bc31d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc31d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc31d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc31d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc31d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc31d-107">Aktualisieren Sie die Eigenschaften eines [GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bc31d-107">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc31d-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="bc31d-108">Prerequisites</span></span>
<span data-ttu-id="bc31d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc31d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bc31d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc31d-111">Permission type</span></span>|<span data-ttu-id="bc31d-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc31d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc31d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc31d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc31d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc31d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bc31d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc31d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc31d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc31d-116">Not supported.</span></span>|
|<span data-ttu-id="bc31d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc31d-117">Application</span></span>|<span data-ttu-id="bc31d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc31d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc31d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc31d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="bc31d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc31d-120">Request headers</span></span>
|<span data-ttu-id="bc31d-121">Header</span><span class="sxs-lookup"><span data-stu-id="bc31d-121">Header</span></span>|<span data-ttu-id="bc31d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bc31d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc31d-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="bc31d-123">Authorization</span></span>|<span data-ttu-id="bc31d-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="bc31d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc31d-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bc31d-125">Accept</span></span>|<span data-ttu-id="bc31d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc31d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc31d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc31d-127">Request body</span></span>
<span data-ttu-id="bc31d-128">Geben Sie im Textkörper Anforderung für das Objekt [GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="bc31d-128">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="bc31d-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="bc31d-129">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="bc31d-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc31d-130">Property</span></span>|<span data-ttu-id="bc31d-131">Typ</span><span class="sxs-lookup"><span data-stu-id="bc31d-131">Type</span></span>|<span data-ttu-id="bc31d-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc31d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc31d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bc31d-133">displayName</span></span>|<span data-ttu-id="bc31d-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc31d-134">String</span></span>|<span data-ttu-id="bc31d-135">Die lokalisierten Anzeigenamen der ADMX-Datei.</span><span class="sxs-lookup"><span data-stu-id="bc31d-135">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="bc31d-136">description</span><span class="sxs-lookup"><span data-stu-id="bc31d-136">description</span></span>|<span data-ttu-id="bc31d-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc31d-137">String</span></span>|<span data-ttu-id="bc31d-138">Die lokalisierte Beschreibung der Richtlinieneinstellungen in der ADMX-Datei.</span><span class="sxs-lookup"><span data-stu-id="bc31d-138">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="bc31d-139">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="bc31d-139">The default value is empty.</span></span>|
|<span data-ttu-id="bc31d-140">languageCodes</span><span class="sxs-lookup"><span data-stu-id="bc31d-140">languageCodes</span></span>|<span data-ttu-id="bc31d-141">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="bc31d-141">String collection</span></span>|<span data-ttu-id="bc31d-142">Die unterstützten Sprachcodes für die ADMX-Datei.</span><span class="sxs-lookup"><span data-stu-id="bc31d-142">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="bc31d-143">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="bc31d-143">targetPrefix</span></span>|<span data-ttu-id="bc31d-144">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc31d-144">String</span></span>|<span data-ttu-id="bc31d-145">Gibt den logischen Namen, der auf den Namespace innerhalb der ADMX-Datei verweist.</span><span class="sxs-lookup"><span data-stu-id="bc31d-145">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="bc31d-146">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="bc31d-146">targetNamespace</span></span>|<span data-ttu-id="bc31d-147">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc31d-147">String</span></span>|<span data-ttu-id="bc31d-148">Gibt den URI verwendet, um den Namespace innerhalb der ADMX-Datei zu identifizieren.</span><span class="sxs-lookup"><span data-stu-id="bc31d-148">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="bc31d-149">policyType</span><span class="sxs-lookup"><span data-stu-id="bc31d-149">policyType</span></span>|[<span data-ttu-id="bc31d-150">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="bc31d-150">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="bc31d-151">Gibt den Typ von Gruppenrichtlinien.</span><span class="sxs-lookup"><span data-stu-id="bc31d-151">Specifies the type of group policy.</span></span> <span data-ttu-id="bc31d-152">Mögliche Werte sind: `admxBacked` und `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="bc31d-152">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="bc31d-153">id</span><span class="sxs-lookup"><span data-stu-id="bc31d-153">id</span></span>|<span data-ttu-id="bc31d-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc31d-154">String</span></span>|<span data-ttu-id="bc31d-155">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bc31d-155">Key of the entity.</span></span>|
|<span data-ttu-id="bc31d-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc31d-156">lastModifiedDateTime</span></span>|<span data-ttu-id="bc31d-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc31d-157">DateTimeOffset</span></span>|<span data-ttu-id="bc31d-158">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="bc31d-158">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="bc31d-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc31d-159">Response</span></span>
<span data-ttu-id="bc31d-160">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="bc31d-160">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc31d-161">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc31d-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc31d-162">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc31d-162">Request</span></span>
<span data-ttu-id="bc31d-163">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc31d-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a><span data-ttu-id="bc31d-164">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc31d-164">Response</span></span>
<span data-ttu-id="bc31d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc31d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 438

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




