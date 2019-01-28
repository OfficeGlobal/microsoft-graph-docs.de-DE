---
title: directoryAudit-Ressourcentyp
description: Diese Ressource stellt Überwachungselemente des Verzeichnisses und seine Sammlung dar.
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0f56dea1b07f0814c4b9f1295498c2555c98a2df
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573158"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="d7802-103">directoryAudit-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d7802-103">directoryAudit resource type</span></span>
<span data-ttu-id="d7802-104">Diese Ressource stellt Überwachungselemente des Verzeichnisses und seine Sammlung dar.</span><span class="sxs-lookup"><span data-stu-id="d7802-104">This resource represents the directory Audit items and its collection</span></span>


## <a name="methods"></a><span data-ttu-id="d7802-105">Methoden</span><span class="sxs-lookup"><span data-stu-id="d7802-105">Methods</span></span>

| <span data-ttu-id="d7802-106">Methode</span><span class="sxs-lookup"><span data-stu-id="d7802-106">Method</span></span>           | <span data-ttu-id="d7802-107">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d7802-107">Return Type</span></span>    |<span data-ttu-id="d7802-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7802-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7802-109">List directoryAudits</span><span class="sxs-lookup"><span data-stu-id="d7802-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="d7802-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="d7802-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="d7802-111">Listet die Überwachungselemente des Verzeichnisses in der Sammlung und ihre Eigenschaften auf.</span><span class="sxs-lookup"><span data-stu-id="d7802-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="d7802-112">Get directoryAudit</span><span class="sxs-lookup"><span data-stu-id="d7802-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="d7802-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="d7802-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="d7802-114">Gibt ein bestimmtes Überwachungselement des Verzeichnisses und seine Eigenschaften an.</span><span class="sxs-lookup"><span data-stu-id="d7802-114">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="d7802-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d7802-115">Properties</span></span>
| <span data-ttu-id="d7802-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d7802-116">Property</span></span>     | <span data-ttu-id="d7802-117">Typ</span><span class="sxs-lookup"><span data-stu-id="d7802-117">Type</span></span>   |<span data-ttu-id="d7802-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d7802-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7802-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="d7802-119">activityDateTime</span></span>|<span data-ttu-id="d7802-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7802-120">DateTimeOffset</span></span>|<span data-ttu-id="d7802-121">Gibt das Datum und die Uhrzeit der Ausführung der Aktivität an.</span><span class="sxs-lookup"><span data-stu-id="d7802-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="d7802-122">Der Zeitstempeltyp liegt immer in UTC-Zeit vor.</span><span class="sxs-lookup"><span data-stu-id="d7802-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d7802-123">Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d7802-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d7802-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="d7802-124">activityDisplayName</span></span>|<span data-ttu-id="d7802-125">String</span><span class="sxs-lookup"><span data-stu-id="d7802-125">String</span></span>|<span data-ttu-id="d7802-126">Gibt den Aktivitätsnamen oder den Vorgangsnamen an (z. B.</span><span class="sxs-lookup"><span data-stu-id="d7802-126">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="d7802-127">"Benutzer erstellen", "Mitglied der Gruppe hinzufügen").</span><span class="sxs-lookup"><span data-stu-id="d7802-127">"Create User", "Add member to group").</span></span> <span data-ttu-id="d7802-128">Eine Liste der protokollierten Aktivitäten finden Sie unter [Azure AD-Aktivitätsliste](https://docs.microsoft.com/de-DE/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span><span class="sxs-lookup"><span data-stu-id="d7802-128">For a list of activities logged,refer to [Azure Ad activity list](https://docs.microsoft.com/de-DE/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="d7802-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="d7802-129">additionalDetails</span></span>|<span data-ttu-id="d7802-130">[keyvalue](keyvalue.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d7802-130">[keyvalue](keyvalue.md) collection</span></span>|<span data-ttu-id="d7802-131">Gibt weitere Details zur Aktivität an.</span><span class="sxs-lookup"><span data-stu-id="d7802-131">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="d7802-132">category</span><span class="sxs-lookup"><span data-stu-id="d7802-132">category</span></span>|<span data-ttu-id="d7802-133">String</span><span class="sxs-lookup"><span data-stu-id="d7802-133">String</span></span>|<span data-ttu-id="d7802-134">Gibt an, auf welche Ressourcenkategorie die Aktivität abzielt.</span><span class="sxs-lookup"><span data-stu-id="d7802-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="d7802-135">(Beispiel: Benutzerverwaltung, Gruppenverwaltung usw.)</span><span class="sxs-lookup"><span data-stu-id="d7802-135">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="d7802-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="d7802-136">correlationId</span></span>| <span data-ttu-id="d7802-137">String (Bezeichner)</span><span class="sxs-lookup"><span data-stu-id="d7802-137">String (identifier)</span></span> |<span data-ttu-id="d7802-138">Gibt eine eindeutige ID an, die bei der Korrelation von Aktivitäten hilft, die sich über verschiedene Dienste erstrecken.</span><span class="sxs-lookup"><span data-stu-id="d7802-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="d7802-139">Kann für die Ablaufverfolgung von Protokollen über Dienste hinweg verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="d7802-139">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="d7802-140">id</span><span class="sxs-lookup"><span data-stu-id="d7802-140">id</span></span>|<span data-ttu-id="d7802-141">String</span><span class="sxs-lookup"><span data-stu-id="d7802-141">String</span></span>| <span data-ttu-id="d7802-142">Gibt die eindeutige ID für die Aktivität an.</span><span class="sxs-lookup"><span data-stu-id="d7802-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="d7802-143">Dies ist eine GUID.</span><span class="sxs-lookup"><span data-stu-id="d7802-143">This is a GUID.</span></span>|
|<span data-ttu-id="d7802-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="d7802-144">initiatedBy</span></span>|[<span data-ttu-id="d7802-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="d7802-145">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="d7802-146">Gibt Informationen zum Benutzer oder der App an, der bzw. die die Aktivität initiiert hat.</span><span class="sxs-lookup"><span data-stu-id="d7802-146">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="d7802-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="d7802-147">loggedByService</span></span>|<span data-ttu-id="d7802-148">String</span><span class="sxs-lookup"><span data-stu-id="d7802-148">String</span></span>|<span data-ttu-id="d7802-149">Gibt Informationen dazu an, welcher Dienst die Aktivität ausgelöst hat (Beispiel: Self-Service-Kennwortverwaltung, Core Directory, B2C, Eingeladene Benutzer, Microsoft Identity Manager, Privileged Identity Management).</span><span class="sxs-lookup"><span data-stu-id="d7802-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="d7802-150">result</span><span class="sxs-lookup"><span data-stu-id="d7802-150">result</span></span>|<span data-ttu-id="d7802-151">string</span><span class="sxs-lookup"><span data-stu-id="d7802-151">string</span></span>| <span data-ttu-id="d7802-152">Gibt das Ergebnis der Aktivität an. Mögliche Werte sind: `success`, `failure`, `timeout`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="d7802-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="d7802-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="d7802-153">resultReason</span></span>|<span data-ttu-id="d7802-154">String</span><span class="sxs-lookup"><span data-stu-id="d7802-154">String</span></span>|<span data-ttu-id="d7802-155">Gibt den Grund für den Fehler an, wenn das Ergebnis "Failure" oder "timeout" ist.</span><span class="sxs-lookup"><span data-stu-id="d7802-155">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>|
|<span data-ttu-id="d7802-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="d7802-156">targetResources</span></span>|<span data-ttu-id="d7802-157">[targetResource](targetresource.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d7802-157">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="d7802-158">Gibt Informationen dazu an, welche Ressource aufgrund der Aktivität geändert wurde.</span><span class="sxs-lookup"><span data-stu-id="d7802-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="d7802-159">Der Zielressourcentyp kann Benutzer, Gerät, Verzeichnis, App, Rolle, Gruppe, Richtlinie oder Andere sein.</span><span class="sxs-lookup"><span data-stu-id="d7802-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="d7802-160">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d7802-160">Relationships</span></span>
<span data-ttu-id="d7802-161">Keine</span><span class="sxs-lookup"><span data-stu-id="d7802-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d7802-162">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d7802-162">JSON representation</span></span>

<span data-ttu-id="d7802-163">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d7802-163">Here is a JSON representation of the resource.</span></span>

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
  "correlationId": "String (identifier)",
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
