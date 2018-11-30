---
title: Ressourcentyp SynchronisationVorlage
description: " Jeder Benutzer kann die Vorlage, um die Standardeinstellungen, einschließlich des Synchronisierungsschemas finden Sie unter abrufen."
ms.openlocfilehash: 90850ad43fdd14fc38ff6ae8cfa97f47806a289d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062232"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="595d3-103">Ressourcentyp SynchronisationVorlage</span><span class="sxs-lookup"><span data-stu-id="595d3-103">synchronizationTemplate resource type</span></span>

> <span data-ttu-id="595d3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="595d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="595d3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="595d3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="595d3-106">Enthält vorkonfigurierte synchronisierungseinstellungen für eine bestimmte Anwendung.</span><span class="sxs-lookup"><span data-stu-id="595d3-106">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="595d3-107">Standardmäßig werden diese Einstellungen für [Synchronisierungsauftrag](synchronization-synchronizationjob.md) verwendet, die auf der Vorlage basiert.</span><span class="sxs-lookup"><span data-stu-id="595d3-107">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="595d3-108">Der Anwendungsentwickler gibt die Vorlage an. Jeder Benutzer kann die Vorlage, um die Standardeinstellungen, einschließlich der [Synchronisierungsschema](synchronization-synchronizationschema.md)finden Sie unter abrufen.</span><span class="sxs-lookup"><span data-stu-id="595d3-108">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="595d3-109">Sie können mehrere Vorlagen für eine Anwendung bereitstellen und eine entsprechende Standardvorlage bestimmen.</span><span class="sxs-lookup"><span data-stu-id="595d3-109">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="595d3-110">Wenn mehrere Vorlagen für die Anwendung verfügbar, den, denen Sie interessiert sind sind, seek dienstanwendungsspezifische Anleitung, um zu bestimmen, welches am besten Ihren Anforderungen entspricht.</span><span class="sxs-lookup"><span data-stu-id="595d3-110">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="595d3-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="595d3-111">Methods</span></span>

| <span data-ttu-id="595d3-112">Methode</span><span class="sxs-lookup"><span data-stu-id="595d3-112">Method</span></span>        | <span data-ttu-id="595d3-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="595d3-113">Return Type</span></span>               | <span data-ttu-id="595d3-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="595d3-114">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="595d3-115">List</span><span class="sxs-lookup"><span data-stu-id="595d3-115">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="595d3-116">[SynchronisationVorlage](synchronization-synchronizationtemplate.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="595d3-116">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="595d3-117">Listenvorlagen Sie für eine Anwendung oder Anwendungsinstanz (Service Principal) verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="595d3-117">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="595d3-118">Get</span><span class="sxs-lookup"><span data-stu-id="595d3-118">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="595d3-119">SynchronisationVorlage</span><span class="sxs-lookup"><span data-stu-id="595d3-119">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="595d3-120">Lesen Sie die Eigenschaften und Beziehungen des **SynchronisationVorlage** -Objekts.</span><span class="sxs-lookup"><span data-stu-id="595d3-120">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="595d3-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="595d3-121">Properties</span></span>

| <span data-ttu-id="595d3-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="595d3-122">Property</span></span>      | <span data-ttu-id="595d3-123">Typ</span><span class="sxs-lookup"><span data-stu-id="595d3-123">Type</span></span>                      | <span data-ttu-id="595d3-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="595d3-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="595d3-125">id</span><span class="sxs-lookup"><span data-stu-id="595d3-125">id</span></span>             |<span data-ttu-id="595d3-126">String</span><span class="sxs-lookup"><span data-stu-id="595d3-126">String</span></span>                     |<span data-ttu-id="595d3-127">Eindeutige Vorlagenbezeichner.</span><span class="sxs-lookup"><span data-stu-id="595d3-127">Unique template identifier.</span></span>|
|<span data-ttu-id="595d3-128">applicationId</span><span class="sxs-lookup"><span data-stu-id="595d3-128">applicationId</span></span>  |<span data-ttu-id="595d3-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="595d3-129">String</span></span>                     |<span data-ttu-id="595d3-130">Bezeichner der Anwendung, zu der diese Vorlage gehört.</span><span class="sxs-lookup"><span data-stu-id="595d3-130">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="595d3-131">default</span><span class="sxs-lookup"><span data-stu-id="595d3-131">default</span></span>        |<span data-ttu-id="595d3-132">Boolesch</span><span class="sxs-lookup"><span data-stu-id="595d3-132">Boolean</span></span>                    |<span data-ttu-id="595d3-133">`true`Wenn diese Vorlage als Standard für die Anwendung empfohlen wird.</span><span class="sxs-lookup"><span data-stu-id="595d3-133">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="595d3-134">description</span><span class="sxs-lookup"><span data-stu-id="595d3-134">description</span></span>    |<span data-ttu-id="595d3-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="595d3-135">String</span></span>                     |<span data-ttu-id="595d3-136">Beschreibung der Vorlage.</span><span class="sxs-lookup"><span data-stu-id="595d3-136">Description of the template.</span></span>|
|<span data-ttu-id="595d3-137">eDiscovery-fähigen</span><span class="sxs-lookup"><span data-stu-id="595d3-137">discoverable</span></span>   |<span data-ttu-id="595d3-138">String</span><span class="sxs-lookup"><span data-stu-id="595d3-138">String</span></span>                     |<span data-ttu-id="595d3-139">`true`Wenn diese Vorlage in der Auflistung der für die Instanz der Anwendung (Service Principal) verfügbaren Vorlagen angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="595d3-139">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="595d3-140">factoryTag</span><span class="sxs-lookup"><span data-stu-id="595d3-140">factoryTag</span></span>     |<span data-ttu-id="595d3-141">String</span><span class="sxs-lookup"><span data-stu-id="595d3-141">String</span></span>                     |<span data-ttu-id="595d3-142">Einer der bekannten Factory Tags durch das Synchronisierungsmodul unterstützt.</span><span class="sxs-lookup"><span data-stu-id="595d3-142">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="595d3-143">Die **FactoryTag** weist dem Synchronisierungsmodul welche-Implementierung, bei der Verarbeitung von Aufträgen, die auf dieser Vorlage basierende.</span><span class="sxs-lookup"><span data-stu-id="595d3-143">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="595d3-144">Metadaten</span><span class="sxs-lookup"><span data-stu-id="595d3-144">metadata</span></span>       |<span data-ttu-id="595d3-145">MetadataEntry-Auflistung</span><span class="sxs-lookup"><span data-stu-id="595d3-145">metadataEntry collection</span></span>   |<span data-ttu-id="595d3-146">Zusätzliche Erweiterungseigenschaften.</span><span class="sxs-lookup"><span data-stu-id="595d3-146">Additional extension properties.</span></span> <span data-ttu-id="595d3-147">Es sei denn, Sie explizit erwähnt, sollte Metadatenwerte nicht geändert werden.</span><span class="sxs-lookup"><span data-stu-id="595d3-147">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="595d3-148">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="595d3-148">Relationships</span></span>
| <span data-ttu-id="595d3-149">Beziehung</span><span class="sxs-lookup"><span data-stu-id="595d3-149">Relationship</span></span>      | <span data-ttu-id="595d3-150">Typ</span><span class="sxs-lookup"><span data-stu-id="595d3-150">Type</span></span>      |<span data-ttu-id="595d3-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="595d3-151">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="595d3-152">Schema</span><span class="sxs-lookup"><span data-stu-id="595d3-152">schema</span></span>             |[<span data-ttu-id="595d3-153">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="595d3-153">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="595d3-154">Synchronisierung-Standardschema für die auf dieser Vorlage basierende Aufträge.</span><span class="sxs-lookup"><span data-stu-id="595d3-154">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="595d3-155">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="595d3-155">JSON representation</span></span>

<span data-ttu-id="595d3-156">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="595d3-156">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->