---
title: GroupPolicyDefinitionValue erstellen
description: Erstellen eines neuen groupPolicyDefinitionValue-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20915d40828e5377502fbbb4f8c1c61a9c963f16
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973110"
---
# <a name="create-grouppolicydefinitionvalue"></a><span data-ttu-id="c77cc-103">GroupPolicyDefinitionValue erstellen</span><span class="sxs-lookup"><span data-stu-id="c77cc-103">Create groupPolicyDefinitionValue</span></span>

> <span data-ttu-id="c77cc-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c77cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c77cc-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="c77cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c77cc-106">Erstellen eines neuen [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="c77cc-106">Create a new [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c77cc-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="c77cc-107">Prerequisites</span></span>
<span data-ttu-id="c77cc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c77cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c77cc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c77cc-110">Permission type</span></span>|<span data-ttu-id="c77cc-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c77cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c77cc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c77cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c77cc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c77cc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c77cc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c77cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c77cc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c77cc-115">Not supported.</span></span>|
|<span data-ttu-id="c77cc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c77cc-116">Application</span></span>|<span data-ttu-id="c77cc-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c77cc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c77cc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c77cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
```

## <a name="request-headers"></a><span data-ttu-id="c77cc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c77cc-119">Request headers</span></span>
|<span data-ttu-id="c77cc-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c77cc-120">Header</span></span>|<span data-ttu-id="c77cc-121">Wert</span><span class="sxs-lookup"><span data-stu-id="c77cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c77cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c77cc-122">Authorization</span></span>|<span data-ttu-id="c77cc-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="c77cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c77cc-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c77cc-124">Accept</span></span>|<span data-ttu-id="c77cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c77cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c77cc-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c77cc-126">Request body</span></span>
<span data-ttu-id="c77cc-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das groupPolicyDefinitionValue-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="c77cc-127">In the request body, supply a JSON representation for the groupPolicyDefinitionValue object.</span></span>

<span data-ttu-id="c77cc-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der groupPolicyDefinitionValue erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="c77cc-128">The following table shows the properties that are required when you create the groupPolicyDefinitionValue.</span></span>

|<span data-ttu-id="c77cc-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c77cc-129">Property</span></span>|<span data-ttu-id="c77cc-130">Typ</span><span class="sxs-lookup"><span data-stu-id="c77cc-130">Type</span></span>|<span data-ttu-id="c77cc-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c77cc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c77cc-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c77cc-132">createdDateTime</span></span>|<span data-ttu-id="c77cc-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c77cc-133">DateTimeOffset</span></span>|<span data-ttu-id="c77cc-134">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="c77cc-134">The date and time the object was created.</span></span>|
|<span data-ttu-id="c77cc-135">aktiviert</span><span class="sxs-lookup"><span data-stu-id="c77cc-135">enabled</span></span>|<span data-ttu-id="c77cc-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="c77cc-136">Boolean</span></span>|<span data-ttu-id="c77cc-137">Aktiviert oder deaktiviert die zugeordnete Gruppenrichtlinien Definition.</span><span class="sxs-lookup"><span data-stu-id="c77cc-137">Enables or disables the associated group policy definition.</span></span>|
|<span data-ttu-id="c77cc-138">configurationType</span><span class="sxs-lookup"><span data-stu-id="c77cc-138">configurationType</span></span>|[<span data-ttu-id="c77cc-139">groupPolicyConfigurationType</span><span class="sxs-lookup"><span data-stu-id="c77cc-139">groupPolicyConfigurationType</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|<span data-ttu-id="c77cc-140">Gibt an, wie der Wert konfiguriert werden soll.</span><span class="sxs-lookup"><span data-stu-id="c77cc-140">Specifies how the value should be configured.</span></span> <span data-ttu-id="c77cc-141">Dabei kann es sich entweder um eine Richtlinie oder eine Präferenz handeln.</span><span class="sxs-lookup"><span data-stu-id="c77cc-141">This can be either as a Policy or as a Preference.</span></span> <span data-ttu-id="c77cc-142">Mögliche Werte: `policy`, `preference`.</span><span class="sxs-lookup"><span data-stu-id="c77cc-142">Possible values are: `policy`, `preference`.</span></span>|
|<span data-ttu-id="c77cc-143">id</span><span class="sxs-lookup"><span data-stu-id="c77cc-143">id</span></span>|<span data-ttu-id="c77cc-144">String</span><span class="sxs-lookup"><span data-stu-id="c77cc-144">String</span></span>|<span data-ttu-id="c77cc-145">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="c77cc-145">Key of the entity.</span></span>|
|<span data-ttu-id="c77cc-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c77cc-146">lastModifiedDateTime</span></span>|<span data-ttu-id="c77cc-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c77cc-147">DateTimeOffset</span></span>|<span data-ttu-id="c77cc-148">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="c77cc-148">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="c77cc-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="c77cc-149">Response</span></span>
<span data-ttu-id="c77cc-150">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="c77cc-150">If successful, this method returns a `201 Created` response code and a [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c77cc-151">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c77cc-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="c77cc-152">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c77cc-152">Request</span></span>
<span data-ttu-id="c77cc-153">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c77cc-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues
Content-type: application/json
Content-length: 126

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "enabled": true,
  "configurationType": "preference"
}
```

### <a name="response"></a><span data-ttu-id="c77cc-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="c77cc-154">Response</span></span>
<span data-ttu-id="c77cc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c77cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




