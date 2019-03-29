---
title: GroupPolicyDefinitionValue aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyDefinitionValue-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34295191a0e0cf2e73b006ecd3b74269027d4bd8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961028"
---
# <a name="update-grouppolicydefinitionvalue"></a><span data-ttu-id="0c314-103">GroupPolicyDefinitionValue aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0c314-103">Update groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="0c314-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0c314-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c314-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="0c314-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c314-106">Aktualisieren der Eigenschaften eines [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c314-106">Update the properties of a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c314-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="0c314-107">Prerequisites</span></span>
<span data-ttu-id="0c314-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c314-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c314-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0c314-110">Permission type</span></span>|<span data-ttu-id="0c314-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0c314-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c314-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0c314-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c314-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c314-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0c314-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0c314-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c314-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c314-115">Not supported.</span></span>|
|<span data-ttu-id="0c314-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0c314-116">Application</span></span>|<span data-ttu-id="0c314-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0c314-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c314-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c314-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/definitionValue
```

## <a name="request-headers"></a><span data-ttu-id="0c314-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0c314-119">Request headers</span></span>
|<span data-ttu-id="0c314-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0c314-120">Header</span></span>|<span data-ttu-id="0c314-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0c314-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c314-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c314-122">Authorization</span></span>|<span data-ttu-id="0c314-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="0c314-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c314-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="0c314-124">Accept</span></span>|<span data-ttu-id="0c314-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c314-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c314-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0c314-126">Request body</span></span>
<span data-ttu-id="0c314-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="0c314-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

<span data-ttu-id="0c314-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0c314-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).</span></span>

|<span data-ttu-id="0c314-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0c314-129">Property</span></span>|<span data-ttu-id="0c314-130">Typ</span><span class="sxs-lookup"><span data-stu-id="0c314-130">Type</span></span>|<span data-ttu-id="0c314-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0c314-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c314-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c314-132">createdDateTime</span></span>|<span data-ttu-id="0c314-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c314-133">DateTimeOffset</span></span>|<span data-ttu-id="0c314-134">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="0c314-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="0c314-135">aktiviert</span><span class="sxs-lookup"><span data-stu-id="0c314-135">enabled</span></span>|<span data-ttu-id="0c314-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c314-136">Boolean</span></span>|<span data-ttu-id="0c314-137">Aktiviert oder deaktiviert die zugeordnete Gruppenrichtlinien Definition.</span><span class="sxs-lookup"><span data-stu-id="0c314-137">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="0c314-138">configurationType</span><span class="sxs-lookup"><span data-stu-id="0c314-138">configurationType</span></span>|[<span data-ttu-id="0c314-139">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="0c314-139">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="0c314-140">Gibt an, wie der Wert konfiguriert werden soll.</span><span class="sxs-lookup"><span data-stu-id="0c314-140">Specifies how the value should be configured.</span></span> <span data-ttu-id="0c314-141">Dabei kann es sich entweder um eine Richtlinie oder eine Präferenz handeln.</span><span class="sxs-lookup"><span data-stu-id="0c314-141">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="0c314-142">Mögliche Werte: `policy`, `preference`.</span><span class="sxs-lookup"><span data-stu-id="0c314-142">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="0c314-143">id</span><span class="sxs-lookup"><span data-stu-id="0c314-143">id</span></span>|<span data-ttu-id="0c314-144">String</span><span class="sxs-lookup"><span data-stu-id="0c314-144">String</span></span>|<span data-ttu-id="0c314-145">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0c314-145">Key of the entity.</span></span>|
|<span data-ttu-id="0c314-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c314-146">lastModifiedDateTime</span></span>|<span data-ttu-id="0c314-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c314-147">DateTimeOffset</span></span>|<span data-ttu-id="0c314-148">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="0c314-148">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="0c314-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c314-149">Response</span></span>
<span data-ttu-id="0c314-150">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="0c314-150">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c314-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0c314-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c314-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0c314-152">Request</span></span>
<span data-ttu-id="0c314-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0c314-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="0c314-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="0c314-154">Response</span></span>
<span data-ttu-id="0c314-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0c314-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "enabled": true,
  "configurationType": "preference",
  "id": "50428918-8918-5042-1889-425018894250",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




