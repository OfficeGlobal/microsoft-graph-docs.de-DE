---
title: Ressourcentyp directoryAudit
description: Diese Ressource stellt die Directory Audit Elemente mit seiner Sammlung
ms.openlocfilehash: 8656bd910cd5b84d7760f973b160d91efe08abe1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27057930"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="00267-103">Ressourcentyp directoryAudit</span><span class="sxs-lookup"><span data-stu-id="00267-103">directoryAudit resource type</span></span>
<span data-ttu-id="00267-104">Diese Ressource stellt die Directory Audit Elemente mit seiner Sammlung</span><span class="sxs-lookup"><span data-stu-id="00267-104">This resource represents the directory Audit items and its collection</span></span>


## <a name="methods"></a><span data-ttu-id="00267-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="00267-105">Methods</span></span>

| <span data-ttu-id="00267-106">Methode</span><span class="sxs-lookup"><span data-stu-id="00267-106">Method</span></span>           | <span data-ttu-id="00267-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="00267-107">Return Type</span></span>    |<span data-ttu-id="00267-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00267-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="00267-109">Liste directoryAudits</span><span class="sxs-lookup"><span data-stu-id="00267-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="00267-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="00267-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="00267-111">Die Directory Audit-Elemente in der Auflistung und deren Eigenschaften aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="00267-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="00267-112">Abrufen von directoryAudit</span><span class="sxs-lookup"><span data-stu-id="00267-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="00267-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="00267-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="00267-114">Rufen Sie ein bestimmtes Verzeichnis Audit-Element und seine Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="00267-114">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="00267-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="00267-115">Properties</span></span>
| <span data-ttu-id="00267-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00267-116">Property</span></span>     | <span data-ttu-id="00267-117">Typ</span><span class="sxs-lookup"><span data-stu-id="00267-117">Type</span></span>   |<span data-ttu-id="00267-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00267-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00267-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="00267-119">activityDateTime</span></span>|<span data-ttu-id="00267-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00267-120">DateTimeOffset</span></span>|<span data-ttu-id="00267-121">Gibt an, das Datum und die Zeit, die die Aktivität ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="00267-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="00267-122">Der Zeitstempel-Typ ist immer in UTC-Zeit.</span><span class="sxs-lookup"><span data-stu-id="00267-122">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="00267-123">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="00267-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="00267-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="00267-124">activityDisplayName</span></span>|<span data-ttu-id="00267-125">String</span><span class="sxs-lookup"><span data-stu-id="00267-125">String</span></span>|<span data-ttu-id="00267-126">Gibt den Namen der Aktivität oder der Name des Vorgangs (z. B.</span><span class="sxs-lookup"><span data-stu-id="00267-126">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="00267-127">"Erstellen von Benutzer", "Add Mitglied der Gruppe").</span><span class="sxs-lookup"><span data-stu-id="00267-127">"Create User", "Add member to group").</span></span> <span data-ttu-id="00267-128">Eine Liste der Aktivitäten protokolliert finden Sie in der [Liste von Azure Ad-Aktivität](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span><span class="sxs-lookup"><span data-stu-id="00267-128">For a list of activities logged,refer to [Azure Ad activity list](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="00267-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="00267-129">additionalDetails</span></span>|<span data-ttu-id="00267-130">[KeyValue](keyvalue.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="00267-130">[keyValue](keyvalue.md) collection</span></span>|<span data-ttu-id="00267-131">Gibt zusätzliche Informationen für die Aktivität an.</span><span class="sxs-lookup"><span data-stu-id="00267-131">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="00267-132">category</span><span class="sxs-lookup"><span data-stu-id="00267-132">category</span></span>|<span data-ttu-id="00267-133">String</span><span class="sxs-lookup"><span data-stu-id="00267-133">String</span></span>|<span data-ttu-id="00267-134">Gibt an, welche Ressourcenkategorie, die von der Aktivität gerichtet ist.</span><span class="sxs-lookup"><span data-stu-id="00267-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="00267-135">(Zum Beispiel: die Verwaltung von usw. Gruppe Management..)</span><span class="sxs-lookup"><span data-stu-id="00267-135">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="00267-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="00267-136">correlationId</span></span>|<span data-ttu-id="00267-137">GUID</span><span class="sxs-lookup"><span data-stu-id="00267-137">GUID</span></span>|<span data-ttu-id="00267-138">Gibt eine eindeutige ID, mit deren Aktivitäten korrelieren, die über verschiedene Dienste erstrecken.</span><span class="sxs-lookup"><span data-stu-id="00267-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="00267-139">Kann in Ablaufprotokolle zwischen Diensten verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="00267-139">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="00267-140">id</span><span class="sxs-lookup"><span data-stu-id="00267-140">id</span></span>|<span data-ttu-id="00267-141">String</span><span class="sxs-lookup"><span data-stu-id="00267-141">String</span></span>| <span data-ttu-id="00267-142">Gibt die eindeutige ID für die Aktivität an.</span><span class="sxs-lookup"><span data-stu-id="00267-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="00267-143">Dies ist eine GUID.</span><span class="sxs-lookup"><span data-stu-id="00267-143">This is a GUID.</span></span>|
|<span data-ttu-id="00267-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="00267-144">initiatedBy</span></span>|[<span data-ttu-id="00267-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="00267-145">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="00267-146">Gibt an, dass Informationen über den Benutzer oder die app die Aktivität initiiert hat.</span><span class="sxs-lookup"><span data-stu-id="00267-146">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="00267-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="00267-147">loggedByService</span></span>|<span data-ttu-id="00267-148">String</span><span class="sxs-lookup"><span data-stu-id="00267-148">String</span></span>|<span data-ttu-id="00267-149">Gibt an, auf dem Dienst die Aktivität initiiert, Informationen (zum Beispiel: Self-Service-Kennwortverwaltung, Core Directory, B2C, Benutzer eingeladen, Microsoft Identity Manager, privilegierten Identity Management.</span><span class="sxs-lookup"><span data-stu-id="00267-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="00267-150">result</span><span class="sxs-lookup"><span data-stu-id="00267-150">result</span></span>|<span data-ttu-id="00267-151">string</span><span class="sxs-lookup"><span data-stu-id="00267-151">string</span></span>| <span data-ttu-id="00267-152">Gibt das Ergebnis der Aktivität an. Mögliche Werte sind: `success`, `failure`, `timeout`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="00267-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="00267-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="00267-153">resultReason</span></span>|<span data-ttu-id="00267-154">String</span><span class="sxs-lookup"><span data-stu-id="00267-154">String</span></span>|<span data-ttu-id="00267-155">Gibt die Ursache für Fehler an, ob das Ergebnis "Fehler" oder "Timeout" ist.</span><span class="sxs-lookup"><span data-stu-id="00267-155">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>|
|<span data-ttu-id="00267-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="00267-156">targetResources</span></span>|<span data-ttu-id="00267-157">[TargetResource](targetresource.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="00267-157">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="00267-158">Gibt Informationen für die Ressource der Aktivitäten geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="00267-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="00267-159">Ressource Zieltyp können Benutzer, Gerät, Directory, App, Rolle, Gruppe, Richtlinie oder andere sein.</span><span class="sxs-lookup"><span data-stu-id="00267-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="00267-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="00267-160">Relationships</span></span>
<span data-ttu-id="00267-161">Keine</span><span class="sxs-lookup"><span data-stu-id="00267-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="00267-162">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="00267-162">JSON representation</span></span>

<span data-ttu-id="00267-163">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="00267-163">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryAudit"
}-->

```json
{
  "activityDateTime": "String (timestamp)",
  "activityDisplayName": "String",
  "additionalDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "category": "String",
  "correlationId": "Guid",
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.auditActivityInitiator"},
  "loggedByService": "String",
  "result": "string",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryAudit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->