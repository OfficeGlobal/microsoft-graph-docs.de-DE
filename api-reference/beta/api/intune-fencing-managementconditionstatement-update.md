---
title: ManagementConditionStatement aktualisieren
description: Aktualisieren Sie die Eigenschaften eines ManagementConditionStatement-Objekts.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 800d40bda342ea23b55e7dc9bf62a99f1e41e3df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935416"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="597c3-103">ManagementConditionStatement aktualisieren</span><span class="sxs-lookup"><span data-stu-id="597c3-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="597c3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="597c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="597c3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="597c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="597c3-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="597c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="597c3-107">Aktualisieren Sie die Eigenschaften eines [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="597c3-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="597c3-108">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="597c3-108">Prerequisites</span></span>
<span data-ttu-id="597c3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="597c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="597c3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="597c3-111">Permission type</span></span>|<span data-ttu-id="597c3-112">Berechtigungen (von der Berechtigung mit den meisten Rechten zu der mit den wenigsten Rechten)</span><span class="sxs-lookup"><span data-stu-id="597c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="597c3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="597c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="597c3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="597c3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="597c3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="597c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="597c3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="597c3-116">Not supported.</span></span>|
|<span data-ttu-id="597c3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="597c3-117">Application</span></span>|<span data-ttu-id="597c3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="597c3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="597c3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="597c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="597c3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="597c3-120">Request headers</span></span>
|<span data-ttu-id="597c3-121">Header</span><span class="sxs-lookup"><span data-stu-id="597c3-121">Header</span></span>|<span data-ttu-id="597c3-122">Wert</span><span class="sxs-lookup"><span data-stu-id="597c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="597c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="597c3-123">Authorization</span></span>|<span data-ttu-id="597c3-124">Bearer&lt;token&gt; erforderlich</span><span class="sxs-lookup"><span data-stu-id="597c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="597c3-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="597c3-125">Accept</span></span>|<span data-ttu-id="597c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="597c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="597c3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="597c3-127">Request body</span></span>
<span data-ttu-id="597c3-128">Geben Sie im Textkörper Anforderung für das Objekt [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) eine JSON-Darstellung.</span><span class="sxs-lookup"><span data-stu-id="597c3-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="597c3-129">In der folgenden Tabelle werden die Eigenschaften gezeigt, die erforderlich sind, wenn Sie die [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)erstellen.</span><span class="sxs-lookup"><span data-stu-id="597c3-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="597c3-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="597c3-130">Property</span></span>|<span data-ttu-id="597c3-131">Typ</span><span class="sxs-lookup"><span data-stu-id="597c3-131">Type</span></span>|<span data-ttu-id="597c3-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="597c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="597c3-133">id</span><span class="sxs-lookup"><span data-stu-id="597c3-133">id</span></span>|<span data-ttu-id="597c3-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="597c3-134">String</span></span>|<span data-ttu-id="597c3-135">Eindeutiger Bezeichner für die Verwaltung Condition-Anweisung.</span><span class="sxs-lookup"><span data-stu-id="597c3-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="597c3-136">System generierten Wert, die beim Erstellen zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="597c3-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="597c3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="597c3-137">displayName</span></span>|<span data-ttu-id="597c3-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="597c3-138">String</span></span>|<span data-ttu-id="597c3-139">Der Administrator definierter Name der Bedingung-Anweisung Management.</span><span class="sxs-lookup"><span data-stu-id="597c3-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="597c3-140">description</span><span class="sxs-lookup"><span data-stu-id="597c3-140">description</span></span>|<span data-ttu-id="597c3-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="597c3-141">String</span></span>|<span data-ttu-id="597c3-142">Der Administrator definiert die Beschreibung der Management Condition-Anweisung.</span><span class="sxs-lookup"><span data-stu-id="597c3-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="597c3-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="597c3-143">createdDateTime</span></span>|<span data-ttu-id="597c3-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="597c3-144">DateTimeOffset</span></span>|<span data-ttu-id="597c3-145">Der Zeitpunkt, an die Management Condition-Anweisung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="597c3-145">The time the management condition statement was created.</span></span> <span data-ttu-id="597c3-146">Generierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="597c3-146">Generated service side.</span></span>|
|<span data-ttu-id="597c3-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="597c3-147">modifiedDateTime</span></span>|<span data-ttu-id="597c3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="597c3-148">DateTimeOffset</span></span>|<span data-ttu-id="597c3-149">Der Zeitpunkt der letzten Änderung die Management Condition-Anweisung.</span><span class="sxs-lookup"><span data-stu-id="597c3-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="597c3-150">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="597c3-150">Updated service side.</span></span>|
|<span data-ttu-id="597c3-151">Ausdruck</span><span class="sxs-lookup"><span data-stu-id="597c3-151">expression</span></span>|[<span data-ttu-id="597c3-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="597c3-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="597c3-153">Die Verwaltung Bedingungsausdruck-Anweisung verwendet, um ausgewertet werden soll, wenn eine Management Anweisung Bedingung wurde aktiviert/deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="597c3-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="597c3-154">eTag</span><span class="sxs-lookup"><span data-stu-id="597c3-154">eTag</span></span>|<span data-ttu-id="597c3-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="597c3-155">String</span></span>|<span data-ttu-id="597c3-156">ETag der Management Condition-Anweisung.</span><span class="sxs-lookup"><span data-stu-id="597c3-156">ETag of the management condition statement.</span></span> <span data-ttu-id="597c3-157">Aktualisierte Service-Seite.</span><span class="sxs-lookup"><span data-stu-id="597c3-157">Updated service side.</span></span>|
|<span data-ttu-id="597c3-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="597c3-158">applicablePlatforms</span></span>|<span data-ttu-id="597c3-159">[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="597c3-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="597c3-160">Die entsprechenden Plattformen für diese Management Condition-Anweisung.</span><span class="sxs-lookup"><span data-stu-id="597c3-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="597c3-161">Dieser Wert ergibt Suche die Management Bedingungen verknüpft ist, für die Verwaltung von Bedingung-Anweisung die Warteschlange gestellt und Schnittpunkt der Plattformen.</span><span class="sxs-lookup"><span data-stu-id="597c3-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="597c3-162">Mögliche Werte sind: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater` und `androidWorkProfile`.</span><span class="sxs-lookup"><span data-stu-id="597c3-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="597c3-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="597c3-163">Response</span></span>
<span data-ttu-id="597c3-164">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine aktualisierte [ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="597c3-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="597c3-165">Beispiel</span><span class="sxs-lookup"><span data-stu-id="597c3-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="597c3-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="597c3-166">Request</span></span>
<span data-ttu-id="597c3-167">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="597c3-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
Content-type: application/json
Content-length: 256

{
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

### <a name="response"></a><span data-ttu-id="597c3-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="597c3-168">Response</span></span>
<span data-ttu-id="597c3-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="597c3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





