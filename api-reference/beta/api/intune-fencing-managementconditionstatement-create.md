---
title: Erstellen von managementConditionStatement
description: Erstellen eines neuen ManagementConditionStatement-Objekts.
ms.openlocfilehash: a01d0233eff9d22b3174a8aa7bd382b9a1266ac2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059205"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="354da-103">Erstellen von managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="354da-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="354da-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="354da-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="354da-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="354da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="354da-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="354da-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="354da-107">Erstellen eines neuen [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="354da-107">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="354da-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="354da-108">Prerequisites</span></span>
<span data-ttu-id="354da-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="354da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="354da-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="354da-111">Permission type</span></span>|<span data-ttu-id="354da-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="354da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="354da-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="354da-113">Delegated (work or school account)</span></span>|<span data-ttu-id="354da-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="354da-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="354da-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="354da-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="354da-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="354da-116">Not supported.</span></span>|
|<span data-ttu-id="354da-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="354da-117">Application</span></span>|<span data-ttu-id="354da-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="354da-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="354da-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="354da-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="354da-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="354da-120">Request headers</span></span>
|<span data-ttu-id="354da-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="354da-121">Header</span></span>|<span data-ttu-id="354da-122">Wert</span><span class="sxs-lookup"><span data-stu-id="354da-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="354da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="354da-123">Authorization</span></span>|<span data-ttu-id="354da-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="354da-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="354da-125">Accept</span><span class="sxs-lookup"><span data-stu-id="354da-125">Accept</span></span>|<span data-ttu-id="354da-126">application/json</span><span class="sxs-lookup"><span data-stu-id="354da-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="354da-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="354da-127">Request body</span></span>
<span data-ttu-id="354da-128">Geben Sie im Textkörper Anforderung für das Objekt ManagementConditionStatement eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="354da-128">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="354da-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die ManagementConditionStatement erstellen.</span><span class="sxs-lookup"><span data-stu-id="354da-129">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="354da-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="354da-130">Property</span></span>|<span data-ttu-id="354da-131">Typ</span><span class="sxs-lookup"><span data-stu-id="354da-131">Type</span></span>|<span data-ttu-id="354da-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="354da-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="354da-133">id</span><span class="sxs-lookup"><span data-stu-id="354da-133">id</span></span>|<span data-ttu-id="354da-134">String</span><span class="sxs-lookup"><span data-stu-id="354da-134">String</span></span>|<span data-ttu-id="354da-135">Eindeutiger Bezeichner für die Verwaltung Condition-Anweisung.</span><span class="sxs-lookup"><span data-stu-id="354da-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="354da-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="354da-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="354da-137">displayName</span><span class="sxs-lookup"><span data-stu-id="354da-137">displayName</span></span>|<span data-ttu-id="354da-138">String</span><span class="sxs-lookup"><span data-stu-id="354da-138">String</span></span>|<span data-ttu-id="354da-139">Der Administrator definierter Name der Bedingung-Anweisung Management.</span><span class="sxs-lookup"><span data-stu-id="354da-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="354da-140">description</span><span class="sxs-lookup"><span data-stu-id="354da-140">description</span></span>|<span data-ttu-id="354da-141">String</span><span class="sxs-lookup"><span data-stu-id="354da-141">String</span></span>|<span data-ttu-id="354da-142">Der Administrator definiert die Beschreibung der Management Condition-Anweisung.</span><span class="sxs-lookup"><span data-stu-id="354da-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="354da-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="354da-143">createdDateTime</span></span>|<span data-ttu-id="354da-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="354da-144">DateTimeOffset</span></span>|<span data-ttu-id="354da-145">Der Zeitpunkt, an die Management Condition-Anweisung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="354da-145">The time the management condition statement was created.</span></span> <span data-ttu-id="354da-146">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="354da-146">Generated service side.</span></span>|
|<span data-ttu-id="354da-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="354da-147">modifiedDateTime</span></span>|<span data-ttu-id="354da-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="354da-148">DateTimeOffset</span></span>|<span data-ttu-id="354da-149">Der Zeitpunkt der letzten Änderung die Management Condition-Anweisung.</span><span class="sxs-lookup"><span data-stu-id="354da-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="354da-150">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="354da-150">Updated service side.</span></span>|
|<span data-ttu-id="354da-151">Ausdruck</span><span class="sxs-lookup"><span data-stu-id="354da-151">expression</span></span>|[<span data-ttu-id="354da-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="354da-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="354da-153">Die Verwaltung Bedingungsausdruck-Anweisung verwendet, um ausgewertet werden soll, wenn eine Management Anweisung Bedingung wurde aktiviert/deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="354da-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="354da-154">eTag</span><span class="sxs-lookup"><span data-stu-id="354da-154">eTag</span></span>|<span data-ttu-id="354da-155">String</span><span class="sxs-lookup"><span data-stu-id="354da-155">String</span></span>|<span data-ttu-id="354da-156">ETag der Management Condition-Anweisung.</span><span class="sxs-lookup"><span data-stu-id="354da-156">ETag of the management condition statement.</span></span> <span data-ttu-id="354da-157">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="354da-157">Updated service side.</span></span>|
|<span data-ttu-id="354da-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="354da-158">applicablePlatforms</span></span>|<span data-ttu-id="354da-159">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="354da-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="354da-160">Die entsprechenden Plattformen für diese Management Condition-Anweisung.</span><span class="sxs-lookup"><span data-stu-id="354da-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="354da-161">Dieser Wert ergibt Suche die Management Bedingungen verknüpft ist, für die Verwaltung von Bedingung-Anweisung die Warteschlange gestellt und Schnittpunkt der Plattformen.</span><span class="sxs-lookup"><span data-stu-id="354da-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="354da-162">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="354da-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="354da-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="354da-163">Response</span></span>
<span data-ttu-id="354da-164">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="354da-164">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="354da-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="354da-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="354da-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="354da-166">Request</span></span>
<span data-ttu-id="354da-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="354da-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="354da-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="354da-168">Response</span></span>
<span data-ttu-id="354da-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="354da-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





