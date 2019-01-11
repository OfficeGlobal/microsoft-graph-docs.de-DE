---
title: managedEBook-Ressourcentyp
description: Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3bf01c2115f4a0224ab09e59a9049324e82fa855
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834188"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="3b5ec-103">managedEBook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3b5ec-103">managedEBook resource type</span></span>

> <span data-ttu-id="3b5ec-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b5ec-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b5ec-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b5ec-107">Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält</span><span class="sxs-lookup"><span data-stu-id="3b5ec-107">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="3b5ec-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="3b5ec-108">Methods</span></span>
|<span data-ttu-id="3b5ec-109">Methode</span><span class="sxs-lookup"><span data-stu-id="3b5ec-109">Method</span></span>|<span data-ttu-id="3b5ec-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="3b5ec-110">Return Type</span></span>|<span data-ttu-id="3b5ec-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b5ec-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3b5ec-112">managedEBooks auflisten</span><span class="sxs-lookup"><span data-stu-id="3b5ec-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="3b5ec-113">[managedEBook](../resources/intune-books-managedebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3b5ec-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="3b5ec-114">Auflisten von Eigenschaften und Beziehungen der [managedEBook](../resources/intune-books-managedebook.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="3b5ec-115">managedEBook abrufen</span><span class="sxs-lookup"><span data-stu-id="3b5ec-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="3b5ec-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="3b5ec-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="3b5ec-117">Lesen von Eigenschaften und Beziehungen des [managedEBook](../resources/intune-books-managedebook.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="3b5ec-118">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="3b5ec-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="3b5ec-119">Keine</span><span class="sxs-lookup"><span data-stu-id="3b5ec-119">None</span></span>|<span data-ttu-id="3b5ec-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="3b5ec-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3b5ec-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3b5ec-121">Properties</span></span>
|<span data-ttu-id="3b5ec-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3b5ec-122">Property</span></span>|<span data-ttu-id="3b5ec-123">Typ</span><span class="sxs-lookup"><span data-stu-id="3b5ec-123">Type</span></span>|<span data-ttu-id="3b5ec-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b5ec-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b5ec-125">id</span><span class="sxs-lookup"><span data-stu-id="3b5ec-125">id</span></span>|<span data-ttu-id="3b5ec-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b5ec-126">String</span></span>|<span data-ttu-id="3b5ec-127">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="3b5ec-127">Key of the entity.</span></span>|
|<span data-ttu-id="3b5ec-128">displayName</span><span class="sxs-lookup"><span data-stu-id="3b5ec-128">displayName</span></span>|<span data-ttu-id="3b5ec-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b5ec-129">String</span></span>|<span data-ttu-id="3b5ec-130">Name des E-Books</span><span class="sxs-lookup"><span data-stu-id="3b5ec-130">Name of the eBook.</span></span>|
|<span data-ttu-id="3b5ec-131">description</span><span class="sxs-lookup"><span data-stu-id="3b5ec-131">description</span></span>|<span data-ttu-id="3b5ec-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b5ec-132">String</span></span>|<span data-ttu-id="3b5ec-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b5ec-133">Description.</span></span>|
|<span data-ttu-id="3b5ec-134">publisher</span><span class="sxs-lookup"><span data-stu-id="3b5ec-134">publisher</span></span>|<span data-ttu-id="3b5ec-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b5ec-135">String</span></span>|<span data-ttu-id="3b5ec-136">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="3b5ec-136">Publisher.</span></span>|
|<span data-ttu-id="3b5ec-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b5ec-137">publishedDateTime</span></span>|<span data-ttu-id="3b5ec-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b5ec-138">DateTimeOffset</span></span>|<span data-ttu-id="3b5ec-139">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="3b5ec-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="3b5ec-140">largeCover</span></span>|[<span data-ttu-id="3b5ec-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3b5ec-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3b5ec-142">Umschlagbild des Buchs</span><span class="sxs-lookup"><span data-stu-id="3b5ec-142">Book cover.</span></span>|
|<span data-ttu-id="3b5ec-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b5ec-143">createdDateTime</span></span>|<span data-ttu-id="3b5ec-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b5ec-144">DateTimeOffset</span></span>|<span data-ttu-id="3b5ec-145">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="3b5ec-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b5ec-146">lastModifiedDateTime</span></span>|<span data-ttu-id="3b5ec-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b5ec-147">DateTimeOffset</span></span>|<span data-ttu-id="3b5ec-148">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="3b5ec-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3b5ec-149">informationUrl</span></span>|<span data-ttu-id="3b5ec-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b5ec-150">String</span></span>|<span data-ttu-id="3b5ec-151">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-151">The more information Url.</span></span>|
|<span data-ttu-id="3b5ec-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3b5ec-152">privacyInformationUrl</span></span>|<span data-ttu-id="3b5ec-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b5ec-153">String</span></span>|<span data-ttu-id="3b5ec-154">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="3b5ec-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b5ec-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="3b5ec-155">Relationships</span></span>
|<span data-ttu-id="3b5ec-156">Beziehung</span><span class="sxs-lookup"><span data-stu-id="3b5ec-156">Relationship</span></span>|<span data-ttu-id="3b5ec-157">Typ</span><span class="sxs-lookup"><span data-stu-id="3b5ec-157">Type</span></span>|<span data-ttu-id="3b5ec-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b5ec-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b5ec-159">categories</span><span class="sxs-lookup"><span data-stu-id="3b5ec-159">categories</span></span>|<span data-ttu-id="3b5ec-160">[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3b5ec-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="3b5ec-161">Die Liste der Kategorien für e-Book.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="3b5ec-162">assignments</span><span class="sxs-lookup"><span data-stu-id="3b5ec-162">assignments</span></span>|<span data-ttu-id="3b5ec-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3b5ec-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="3b5ec-164">Die Liste der Zuweisungen für dieses E-Book.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="3b5ec-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="3b5ec-165">installSummary</span></span>|[<span data-ttu-id="3b5ec-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3b5ec-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="3b5ec-167">Die Installationszusammenfassung für die mobile App.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="3b5ec-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="3b5ec-168">deviceStates</span></span>|<span data-ttu-id="3b5ec-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3b5ec-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="3b5ec-170">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="3b5ec-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="3b5ec-171">userStateSummary</span></span>|<span data-ttu-id="3b5ec-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="3b5ec-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="3b5ec-173">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b5ec-174">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3b5ec-174">JSON Representation</span></span>
<span data-ttu-id="3b5ec-175">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3b5ec-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```





