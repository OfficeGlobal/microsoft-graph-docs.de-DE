---
title: managedEBook-Ressourcentyp
description: Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08bd5cc6f5630aca0ff5b35c5590875d259ad294
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422047"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="d6220-103">managedEBook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d6220-103">managedEBook resource type</span></span>

> <span data-ttu-id="d6220-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="d6220-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d6220-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d6220-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6220-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d6220-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6220-107">Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält</span><span class="sxs-lookup"><span data-stu-id="d6220-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="d6220-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="d6220-108">Methods</span></span>
|<span data-ttu-id="d6220-109">Methode</span><span class="sxs-lookup"><span data-stu-id="d6220-109">Method</span></span>|<span data-ttu-id="d6220-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d6220-110">Return Type</span></span>|<span data-ttu-id="d6220-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6220-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d6220-112">managedEBooks auflisten</span><span class="sxs-lookup"><span data-stu-id="d6220-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="d6220-113">[managedEBook](../resources/intune-books-managedebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d6220-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="d6220-114">Auflisten von Eigenschaften und Beziehungen der [managedEBook](../resources/intune-books-managedebook.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="d6220-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="d6220-115">managedEBook abrufen</span><span class="sxs-lookup"><span data-stu-id="d6220-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="d6220-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="d6220-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="d6220-117">Lesen von Eigenschaften und Beziehungen des [managedEBook](../resources/intune-books-managedebook.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d6220-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="d6220-118">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="d6220-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="d6220-119">Keine</span><span class="sxs-lookup"><span data-stu-id="d6220-119">None</span></span>|<span data-ttu-id="d6220-120">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d6220-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d6220-121">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d6220-121">Properties</span></span>
|<span data-ttu-id="d6220-122">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d6220-122">Property</span></span>|<span data-ttu-id="d6220-123">Typ</span><span class="sxs-lookup"><span data-stu-id="d6220-123">Type</span></span>|<span data-ttu-id="d6220-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6220-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6220-125">id</span><span class="sxs-lookup"><span data-stu-id="d6220-125">id</span></span>|<span data-ttu-id="d6220-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d6220-126">String</span></span>|<span data-ttu-id="d6220-127">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="d6220-127">Key of the entity.</span></span>|
|<span data-ttu-id="d6220-128">displayName</span><span class="sxs-lookup"><span data-stu-id="d6220-128">displayName</span></span>|<span data-ttu-id="d6220-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d6220-129">String</span></span>|<span data-ttu-id="d6220-130">Name des E-Books</span><span class="sxs-lookup"><span data-stu-id="d6220-130">Name of the eBook.</span></span>|
|<span data-ttu-id="d6220-131">description</span><span class="sxs-lookup"><span data-stu-id="d6220-131">description</span></span>|<span data-ttu-id="d6220-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d6220-132">String</span></span>|<span data-ttu-id="d6220-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6220-133">Description.</span></span>|
|<span data-ttu-id="d6220-134">publisher</span><span class="sxs-lookup"><span data-stu-id="d6220-134">publisher</span></span>|<span data-ttu-id="d6220-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d6220-135">String</span></span>|<span data-ttu-id="d6220-136">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="d6220-136">Publisher.</span></span>|
|<span data-ttu-id="d6220-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6220-137">publishedDateTime</span></span>|<span data-ttu-id="d6220-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6220-138">DateTimeOffset</span></span>|<span data-ttu-id="d6220-139">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="d6220-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="d6220-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="d6220-140">largeCover</span></span>|[<span data-ttu-id="d6220-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d6220-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d6220-142">Umschlagbild des Buchs</span><span class="sxs-lookup"><span data-stu-id="d6220-142">Book cover.</span></span>|
|<span data-ttu-id="d6220-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6220-143">createdDateTime</span></span>|<span data-ttu-id="d6220-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6220-144">DateTimeOffset</span></span>|<span data-ttu-id="d6220-145">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="d6220-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="d6220-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6220-146">lastModifiedDateTime</span></span>|<span data-ttu-id="d6220-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6220-147">DateTimeOffset</span></span>|<span data-ttu-id="d6220-148">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="d6220-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="d6220-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d6220-149">informationUrl</span></span>|<span data-ttu-id="d6220-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d6220-150">String</span></span>|<span data-ttu-id="d6220-151">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="d6220-151">The more information Url.</span></span>|
|<span data-ttu-id="d6220-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d6220-152">privacyInformationUrl</span></span>|<span data-ttu-id="d6220-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d6220-153">String</span></span>|<span data-ttu-id="d6220-154">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="d6220-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6220-155">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d6220-155">Relationships</span></span>
|<span data-ttu-id="d6220-156">Beziehung</span><span class="sxs-lookup"><span data-stu-id="d6220-156">Relationship</span></span>|<span data-ttu-id="d6220-157">Typ</span><span class="sxs-lookup"><span data-stu-id="d6220-157">Type</span></span>|<span data-ttu-id="d6220-158">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d6220-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6220-159">categories</span><span class="sxs-lookup"><span data-stu-id="d6220-159">categories</span></span>|<span data-ttu-id="d6220-160">[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="d6220-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="d6220-161">Die Liste der Kategorien für e-Book.</span><span class="sxs-lookup"><span data-stu-id="d6220-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="d6220-162">assignments</span><span class="sxs-lookup"><span data-stu-id="d6220-162">assignments</span></span>|<span data-ttu-id="d6220-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d6220-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="d6220-164">Die Liste der Zuweisungen für dieses E-Book.</span><span class="sxs-lookup"><span data-stu-id="d6220-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="d6220-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="d6220-165">installSummary</span></span>|[<span data-ttu-id="d6220-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d6220-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="d6220-167">Die Installationszusammenfassung für die mobile App.</span><span class="sxs-lookup"><span data-stu-id="d6220-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="d6220-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="d6220-168">deviceStates</span></span>|<span data-ttu-id="d6220-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d6220-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="d6220-170">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="d6220-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="d6220-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="d6220-171">userStateSummary</span></span>|<span data-ttu-id="d6220-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d6220-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="d6220-173">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="d6220-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6220-174">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d6220-174">JSON Representation</span></span>
<span data-ttu-id="d6220-175">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d6220-175">Here is a JSON representation of the resource.</span></span>
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




