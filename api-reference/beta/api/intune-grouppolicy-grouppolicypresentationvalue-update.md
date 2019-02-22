---
title: GroupPolicyPresentationValue aktualisieren
description: Aktualisieren der Eigenschaften eines groupPolicyPresentationValue-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b4ce9b5c515a6e765e1e87cceca3dd98358c57d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152094"
---
# <a name="update-grouppolicypresentationvalue"></a><span data-ttu-id="e33af-103">GroupPolicyPresentationValue aktualisieren</span><span class="sxs-lookup"><span data-stu-id="e33af-103">Update groupPolicyPresentationValue</span></span>

> <span data-ttu-id="e33af-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e33af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e33af-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="e33af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e33af-106">Aktualisieren der Eigenschaften eines [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="e33af-106">Update the properties of a [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e33af-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="e33af-107">Prerequisites</span></span>
<span data-ttu-id="e33af-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e33af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e33af-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e33af-110">Permission type</span></span>|<span data-ttu-id="e33af-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e33af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e33af-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e33af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e33af-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e33af-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e33af-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e33af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e33af-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e33af-115">Not supported.</span></span>|
|<span data-ttu-id="e33af-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e33af-116">Application</span></span>|<span data-ttu-id="e33af-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e33af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e33af-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e33af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
```

## <a name="request-headers"></a><span data-ttu-id="e33af-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e33af-119">Request headers</span></span>
|<span data-ttu-id="e33af-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e33af-120">Header</span></span>|<span data-ttu-id="e33af-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e33af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e33af-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e33af-122">Authorization</span></span>|<span data-ttu-id="e33af-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="e33af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e33af-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="e33af-124">Accept</span></span>|<span data-ttu-id="e33af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e33af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e33af-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e33af-126">Request body</span></span>
<span data-ttu-id="e33af-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekt an.</span><span class="sxs-lookup"><span data-stu-id="e33af-127">In the request body, supply a JSON representation for the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object.</span></span>

<span data-ttu-id="e33af-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="e33af-128">The following table shows the properties that are required when you create the [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).</span></span>

|<span data-ttu-id="e33af-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e33af-129">Property</span></span>|<span data-ttu-id="e33af-130">Typ</span><span class="sxs-lookup"><span data-stu-id="e33af-130">Type</span></span>|<span data-ttu-id="e33af-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e33af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e33af-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e33af-132">lastModifiedDateTime</span></span>|<span data-ttu-id="e33af-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e33af-133">DateTimeOffset</span></span>|<span data-ttu-id="e33af-134">Datum und Uhrzeit der letzten Änderung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e33af-134">The date and time the object was last modified.</span></span>|
|<span data-ttu-id="e33af-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e33af-135">createdDateTime</span></span>|<span data-ttu-id="e33af-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e33af-136">DateTimeOffset</span></span>|<span data-ttu-id="e33af-137">Das Datum und die Uhrzeit der Erstellung des Objekts.</span><span class="sxs-lookup"><span data-stu-id="e33af-137">The date and time the object was created.</span></span>|
|<span data-ttu-id="e33af-138">id</span><span class="sxs-lookup"><span data-stu-id="e33af-138">id</span></span>|<span data-ttu-id="e33af-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e33af-139">String</span></span>|<span data-ttu-id="e33af-140">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="e33af-140">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="e33af-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="e33af-141">Response</span></span>
<span data-ttu-id="e33af-142">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein aktualisiertes [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="e33af-142">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e33af-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e33af-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="e33af-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e33af-144">Request</span></span>
<span data-ttu-id="e33af-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e33af-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}
Content-type: application/json
Content-length: 70

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue"
}
```

### <a name="response"></a><span data-ttu-id="e33af-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="e33af-146">Response</span></span>
<span data-ttu-id="e33af-p102">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e33af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "id": "8132eaab-eaab-8132-abea-3281abea3281"
}
```




