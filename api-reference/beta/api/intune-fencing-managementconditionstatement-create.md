---
title: ManagementConditionStatement erstellen
description: Erstellen eines neuen managementConditionStatement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f19cef2899a11a57b06590c006de2181865a9d45
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156861"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="d0bb7-103">ManagementConditionStatement erstellen</span><span class="sxs-lookup"><span data-stu-id="d0bb7-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="d0bb7-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0bb7-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0bb7-106">Erstellen eines neuen [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-106">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0bb7-107">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="d0bb7-107">Prerequisites</span></span>
<span data-ttu-id="d0bb7-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="d0bb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d0bb7-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d0bb7-110">Permission type</span></span>|<span data-ttu-id="d0bb7-111">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d0bb7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0bb7-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d0bb7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0bb7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0bb7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0bb7-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d0bb7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0bb7-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d0bb7-115">Not supported.</span></span>|
|<span data-ttu-id="d0bb7-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d0bb7-116">Application</span></span>|<span data-ttu-id="d0bb7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d0bb7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0bb7-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0bb7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="d0bb7-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d0bb7-119">Request headers</span></span>
|<span data-ttu-id="d0bb7-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d0bb7-120">Header</span></span>|<span data-ttu-id="d0bb7-121">Wert</span><span class="sxs-lookup"><span data-stu-id="d0bb7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0bb7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0bb7-122">Authorization</span></span>|<span data-ttu-id="d0bb7-123">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="d0bb7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0bb7-124">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d0bb7-124">Accept</span></span>|<span data-ttu-id="d0bb7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0bb7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0bb7-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d0bb7-126">Request body</span></span>
<span data-ttu-id="d0bb7-127">Geben Sie im Anforderungstext eine JSON-Darstellung für das managementConditionStatement-Objekt an.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-127">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="d0bb7-128">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen der managementConditionStatement erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-128">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="d0bb7-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d0bb7-129">Property</span></span>|<span data-ttu-id="d0bb7-130">Typ</span><span class="sxs-lookup"><span data-stu-id="d0bb7-130">Type</span></span>|<span data-ttu-id="d0bb7-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d0bb7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0bb7-132">id</span><span class="sxs-lookup"><span data-stu-id="d0bb7-132">id</span></span>|<span data-ttu-id="d0bb7-133">string</span><span class="sxs-lookup"><span data-stu-id="d0bb7-133">String</span></span>|<span data-ttu-id="d0bb7-134">Eindeutiger Bezeichner für die Verwaltungs Bedingungsanweisung.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-134">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="d0bb7-135">Vom System generierter Wert, der bei der Erstellung zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="d0bb7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d0bb7-136">displayName</span></span>|<span data-ttu-id="d0bb7-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0bb7-137">String</span></span>|<span data-ttu-id="d0bb7-138">Der vom Administrator definierte Name der Verwaltungs Bedingungsanweisung.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-138">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="d0bb7-139">description</span><span class="sxs-lookup"><span data-stu-id="d0bb7-139">description</span></span>|<span data-ttu-id="d0bb7-140">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0bb7-140">String</span></span>|<span data-ttu-id="d0bb7-141">Die vom Administrator definierte Beschreibung der Verwaltungs Bedingungsanweisung.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-141">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="d0bb7-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0bb7-142">createdDateTime</span></span>|<span data-ttu-id="d0bb7-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0bb7-143">DateTimeOffset</span></span>|<span data-ttu-id="d0bb7-144">Der Zeitpunkt, zu dem die Verwaltungs Bedingungsanweisung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-144">The time the management condition statement was created.</span></span> <span data-ttu-id="d0bb7-145">Generierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-145">Generated service side.</span></span>|
|<span data-ttu-id="d0bb7-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0bb7-146">modifiedDateTime</span></span>|<span data-ttu-id="d0bb7-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0bb7-147">DateTimeOffset</span></span>|<span data-ttu-id="d0bb7-148">Der Zeitpunkt, zu dem die Anweisung für die Verwaltungsbedingung zuletzt geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-148">The time the management condition statement was last modified.</span></span> <span data-ttu-id="d0bb7-149">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-149">Updated service side.</span></span>|
|<span data-ttu-id="d0bb7-150">Ausdruck</span><span class="sxs-lookup"><span data-stu-id="d0bb7-150">expression</span></span>|[<span data-ttu-id="d0bb7-151">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="d0bb7-151">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="d0bb7-152">Der Ausdruck der Verwaltungs Bedingungsanweisung, mit dem ausgewertet wird, ob eine Anweisung für die Verwaltungsbedingung aktiviert/deaktiviert wurde.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-152">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="d0bb7-153">eTag</span><span class="sxs-lookup"><span data-stu-id="d0bb7-153">eTag</span></span>|<span data-ttu-id="d0bb7-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d0bb7-154">String</span></span>|<span data-ttu-id="d0bb7-155">ETag der Verwaltungs Bedingungsanweisung.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-155">ETag of the management condition statement.</span></span> <span data-ttu-id="d0bb7-156">Aktualisierte Dienstseite.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-156">Updated service side.</span></span>|
|<span data-ttu-id="d0bb7-157">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="d0bb7-157">applicablePlatforms</span></span>|<span data-ttu-id="d0bb7-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Sammlung</span><span class="sxs-lookup"><span data-stu-id="d0bb7-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="d0bb7-159">Die entsprechenden Plattformen für diese Verwaltungs Bedingungsanweisung.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-159">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="d0bb7-160">Dies wird berechnet anhand der Verwaltungsbedingungen, die mit der Verwaltungs Bedingungsanweisung verbunden sind, und dem Auffinden der Schnittstelle der entsprechenden Plattformen.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-160">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="d0bb7-161">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-161">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="d0bb7-162">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0bb7-162">Response</span></span>
<span data-ttu-id="d0bb7-163">Bei erfolgreicher Ausführung gibt diese Methode den `201 Created` Antwortcode und ein [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-163">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0bb7-164">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d0bb7-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0bb7-165">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d0bb7-165">Request</span></span>
<span data-ttu-id="d0bb7-166">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d0bb7-167">Antwort</span><span class="sxs-lookup"><span data-stu-id="d0bb7-167">Response</span></span>
<span data-ttu-id="d0bb7-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d0bb7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```




