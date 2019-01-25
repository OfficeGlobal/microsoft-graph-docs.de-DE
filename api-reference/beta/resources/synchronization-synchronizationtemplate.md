---
title: Ressourcentyp SynchronisationVorlage
description: " Jeder Benutzer kann die Vorlage, um die Standardeinstellungen, einschließlich des Synchronisierungsschemas finden Sie unter abrufen."
localization_priority: Normal
ms.openlocfilehash: 75df13d55cfb58aafe8a751279e103424aa29367
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516553"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="50709-103">Ressourcentyp SynchronisationVorlage</span><span class="sxs-lookup"><span data-stu-id="50709-103">synchronizationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50709-104">Enthält vorkonfigurierte synchronisierungseinstellungen für eine bestimmte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="50709-104">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="50709-105">Standardmäßig werden diese Einstellungen für [Synchronisierungsauftrag](synchronization-synchronizationjob.md) verwendet, die auf der Vorlage basiert.</span><span class="sxs-lookup"><span data-stu-id="50709-105">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="50709-106">Der Anwendungsentwickler gibt die Vorlage an. Jeder Benutzer kann die Vorlage, um die Standardeinstellungen, einschließlich der [Synchronisierungsschema](synchronization-synchronizationschema.md)finden Sie unter abrufen.</span><span class="sxs-lookup"><span data-stu-id="50709-106">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="50709-107">Sie können mehrere Vorlagen für eine Anwendung bereitstellen und eine entsprechende Standardvorlage bestimmen.</span><span class="sxs-lookup"><span data-stu-id="50709-107">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="50709-108">Wenn mehrere Vorlagen für die Anwendung verfügbar, den, denen Sie interessiert sind sind, seek dienstanwendungsspezifische Anleitung, um zu bestimmen, welches am besten Ihren Anforderungen entspricht.</span><span class="sxs-lookup"><span data-stu-id="50709-108">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="50709-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="50709-109">Methods</span></span>

| <span data-ttu-id="50709-110">Methode</span><span class="sxs-lookup"><span data-stu-id="50709-110">Method</span></span>        | <span data-ttu-id="50709-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="50709-111">Return Type</span></span>               | <span data-ttu-id="50709-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50709-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="50709-113">List</span><span class="sxs-lookup"><span data-stu-id="50709-113">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="50709-114">[SynchronisationVorlage](synchronization-synchronizationtemplate.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="50709-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="50709-115">Listenvorlagen Sie für eine Anwendung oder Anwendungsinstanz (Service Principal) verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="50709-115">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="50709-116">Get</span><span class="sxs-lookup"><span data-stu-id="50709-116">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="50709-117">SynchronisationVorlage</span><span class="sxs-lookup"><span data-stu-id="50709-117">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="50709-118">Lesen Sie die Eigenschaften und Beziehungen des **SynchronisationVorlage** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="50709-118">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="50709-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="50709-119">Properties</span></span>

| <span data-ttu-id="50709-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="50709-120">Property</span></span>      | <span data-ttu-id="50709-121">Typ</span><span class="sxs-lookup"><span data-stu-id="50709-121">Type</span></span>                      | <span data-ttu-id="50709-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50709-122">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="50709-123">id</span><span class="sxs-lookup"><span data-stu-id="50709-123">id</span></span>             |<span data-ttu-id="50709-124">string</span><span class="sxs-lookup"><span data-stu-id="50709-124">String</span></span>                     |<span data-ttu-id="50709-125">Eindeutige Vorlagenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="50709-125">Unique template identifier.</span></span>|
|<span data-ttu-id="50709-126">applicationId</span><span class="sxs-lookup"><span data-stu-id="50709-126">applicationId</span></span>  |<span data-ttu-id="50709-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="50709-127">String</span></span>                     |<span data-ttu-id="50709-128">Bezeichner der Anwendung, zu der diese Vorlage gehört.</span><span class="sxs-lookup"><span data-stu-id="50709-128">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="50709-129">default</span><span class="sxs-lookup"><span data-stu-id="50709-129">default</span></span>        |<span data-ttu-id="50709-130">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="50709-130">Boolean</span></span>                    |<span data-ttu-id="50709-131">`true`Wenn diese Vorlage als Standard für die Anwendung empfohlen wird.</span><span class="sxs-lookup"><span data-stu-id="50709-131">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="50709-132">description</span><span class="sxs-lookup"><span data-stu-id="50709-132">description</span></span>    |<span data-ttu-id="50709-133">String</span><span class="sxs-lookup"><span data-stu-id="50709-133">String</span></span>                     |<span data-ttu-id="50709-134">Beschreibung der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="50709-134">Description of the template.</span></span>|
|<span data-ttu-id="50709-135">eDiscovery-fähigen</span><span class="sxs-lookup"><span data-stu-id="50709-135">discoverable</span></span>   |<span data-ttu-id="50709-136">String</span><span class="sxs-lookup"><span data-stu-id="50709-136">String</span></span>                     |<span data-ttu-id="50709-137">`true`Wenn diese Vorlage in der Auflistung der für die Instanz der Anwendung (Service Principal) verfügbaren Vorlagen angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="50709-137">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="50709-138">factoryTag</span><span class="sxs-lookup"><span data-stu-id="50709-138">factoryTag</span></span>     |<span data-ttu-id="50709-139">String</span><span class="sxs-lookup"><span data-stu-id="50709-139">String</span></span>                     |<span data-ttu-id="50709-140">Einer der bekannten Factory Tags durch das Synchronisierungsmodul unterstützt.</span><span class="sxs-lookup"><span data-stu-id="50709-140">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="50709-141">Die **FactoryTag** weist dem Synchronisierungsmodul welche-Implementierung, bei der Verarbeitung von Aufträgen, die auf dieser Vorlage basierende.</span><span class="sxs-lookup"><span data-stu-id="50709-141">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="50709-142">$metadata</span><span class="sxs-lookup"><span data-stu-id="50709-142">metadata</span></span>       |<span data-ttu-id="50709-143">MetadataEntry-Auflistung</span><span class="sxs-lookup"><span data-stu-id="50709-143">metadataEntry collection</span></span>   |<span data-ttu-id="50709-144">Zusätzliche Erweiterungseigenschaften.</span><span class="sxs-lookup"><span data-stu-id="50709-144">Additional extension properties.</span></span> <span data-ttu-id="50709-145">Es sei denn, Sie explizit erwähnt, sollte Metadatenwerte nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="50709-145">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50709-146">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="50709-146">Relationships</span></span>
| <span data-ttu-id="50709-147">Beziehung</span><span class="sxs-lookup"><span data-stu-id="50709-147">Relationship</span></span>      | <span data-ttu-id="50709-148">Typ</span><span class="sxs-lookup"><span data-stu-id="50709-148">Type</span></span>      |<span data-ttu-id="50709-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="50709-149">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="50709-150">Schema</span><span class="sxs-lookup"><span data-stu-id="50709-150">schema</span></span>             |[<span data-ttu-id="50709-151">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="50709-151">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="50709-152">Synchronisierung-Standardschema für die auf dieser Vorlage basierende Aufträge.</span><span class="sxs-lookup"><span data-stu-id="50709-152">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50709-153">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="50709-153">JSON representation</span></span>

<span data-ttu-id="50709-154">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="50709-154">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}-->

```json
{
  "applicationId": "String (identifier)",
  "default": true,
  "description": "String",
  "discoverable": true,
  "factoryTag": "String",
  "id": "String (identifier)",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "schema": {"@odata.type": "microsoft.graph.synchronizationSchema"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
