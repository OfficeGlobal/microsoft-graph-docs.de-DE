---
title: GroupPolicyDefinitionFile aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyDefinitionFile-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e204382f9237428b30362f7464264f732e13541a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169412"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="42648-103">GroupPolicyDefinitionFile aktualisieren</span><span class="sxs-lookup"><span data-stu-id="42648-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="42648-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="42648-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42648-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="42648-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42648-106">Aktualisieren der Eigenschaften eines [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="42648-106">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42648-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="42648-107">Prerequisites</span></span>
<span data-ttu-id="42648-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="42648-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="42648-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="42648-110">Permission type</span></span>|<span data-ttu-id="42648-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="42648-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42648-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="42648-112">Delegated (work or school account)</span></span>|<span data-ttu-id="42648-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42648-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="42648-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="42648-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42648-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42648-115">Not supported.</span></span>|
|<span data-ttu-id="42648-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="42648-116">Application</span></span>|<span data-ttu-id="42648-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="42648-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42648-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="42648-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="42648-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="42648-119">Request headers</span></span>
|<span data-ttu-id="42648-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="42648-120">Header</span></span>|<span data-ttu-id="42648-121">Wert</span><span class="sxs-lookup"><span data-stu-id="42648-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42648-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="42648-122">Authorization</span></span>|<span data-ttu-id="42648-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="42648-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42648-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="42648-124">Accept</span></span>|<span data-ttu-id="42648-125">application/json</span><span class="sxs-lookup"><span data-stu-id="42648-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42648-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="42648-126">Request body</span></span>
<span data-ttu-id="42648-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="42648-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="42648-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="42648-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="42648-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="42648-129">Property</span></span>|<span data-ttu-id="42648-130">Typ</span><span class="sxs-lookup"><span data-stu-id="42648-130">Type</span></span>|<span data-ttu-id="42648-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="42648-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42648-132">displayName</span><span class="sxs-lookup"><span data-stu-id="42648-132">displayName</span></span>|<span data-ttu-id="42648-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="42648-133">String</span></span>|<span data-ttu-id="42648-134">Der lokalisierte Anzeigename der ADMX-Datei.</span><span class="sxs-lookup"><span data-stu-id="42648-134">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="42648-135">description</span><span class="sxs-lookup"><span data-stu-id="42648-135">description</span></span>|<span data-ttu-id="42648-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="42648-136">String</span></span>|<span data-ttu-id="42648-137">Die lokalisierte Beschreibung der Richtlinieneinstellungen in der ADMX-Datei.</span><span class="sxs-lookup"><span data-stu-id="42648-137">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="42648-138">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="42648-138">The default value is empty.</span></span>|
|<span data-ttu-id="42648-139">languageCodes</span><span class="sxs-lookup"><span data-stu-id="42648-139">languageCodes</span></span>|<span data-ttu-id="42648-140">String collection</span><span class="sxs-lookup"><span data-stu-id="42648-140">String collection</span></span>|<span data-ttu-id="42648-141">Die unterstützten Sprachcodes für die ADMX-Datei.</span><span class="sxs-lookup"><span data-stu-id="42648-141">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="42648-142">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="42648-142">targetPrefix</span></span>|<span data-ttu-id="42648-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="42648-143">String</span></span>|<span data-ttu-id="42648-144">Gibt den logischen Namen an, der auf den Namespace innerhalb der ADMX-Datei verweist.</span><span class="sxs-lookup"><span data-stu-id="42648-144">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="42648-145">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="42648-145">targetNamespace</span></span>|<span data-ttu-id="42648-146">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="42648-146">String</span></span>|<span data-ttu-id="42648-147">Gibt den URI an, der zum Identifizieren des Namespaces innerhalb der ADMX-Datei verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="42648-147">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="42648-148">policyType</span><span class="sxs-lookup"><span data-stu-id="42648-148">policyType</span></span>|[<span data-ttu-id="42648-149">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="42648-149">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="42648-150">Gibt den Typ der Gruppenrichtlinie an.</span><span class="sxs-lookup"><span data-stu-id="42648-150">Specifies the type of group policy.</span></span> <span data-ttu-id="42648-151">Mögliche Werte sind: `admxBacked` und `admxIngested`.</span><span class="sxs-lookup"><span data-stu-id="42648-151">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="42648-152">id</span><span class="sxs-lookup"><span data-stu-id="42648-152">id</span></span>|<span data-ttu-id="42648-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="42648-153">String</span></span>|<span data-ttu-id="42648-154">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="42648-154">Key of the entity.</span></span>|
|<span data-ttu-id="42648-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="42648-155">lastModifiedDateTime</span></span>|<span data-ttu-id="42648-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42648-156">DateTimeOffset</span></span>|<span data-ttu-id="42648-157">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="42648-157">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="42648-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="42648-158">Response</span></span>
<span data-ttu-id="42648-159">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="42648-159">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42648-160">Beispiel</span><span class="sxs-lookup"><span data-stu-id="42648-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="42648-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="42648-161">Request</span></span>
<span data-ttu-id="42648-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="42648-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="42648-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="42648-163">Response</span></span>
<span data-ttu-id="42648-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="42648-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




