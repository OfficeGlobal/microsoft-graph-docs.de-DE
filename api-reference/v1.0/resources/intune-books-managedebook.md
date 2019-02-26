---
title: managedEBook-Ressourcentyp
description: Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae6151c23bf05b076ade441f908a2810c80f45ed
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253463"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="561d7-103">managedEBook-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="561d7-103">managedEBook resource type</span></span>

> <span data-ttu-id="561d7-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="561d7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="561d7-105">Eine abstrakte Klasse, die die grundlegenden Eigenschaften des verwalteten eBooks enthält</span><span class="sxs-lookup"><span data-stu-id="561d7-105">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="561d7-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="561d7-106">Methods</span></span>
|<span data-ttu-id="561d7-107">Methode</span><span class="sxs-lookup"><span data-stu-id="561d7-107">Method</span></span>|<span data-ttu-id="561d7-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="561d7-108">Return Type</span></span>|<span data-ttu-id="561d7-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="561d7-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="561d7-110">managedEBooks auflisten</span><span class="sxs-lookup"><span data-stu-id="561d7-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="561d7-111">[managedEBook](../resources/intune-books-managedebook.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="561d7-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="561d7-112">Auflisten von Eigenschaften und Beziehungen der [managedEBook](../resources/intune-books-managedebook.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="561d7-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="561d7-113">managedEBook abrufen</span><span class="sxs-lookup"><span data-stu-id="561d7-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="561d7-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="561d7-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="561d7-115">Lesen von Eigenschaften und Beziehungen des [managedEBook](../resources/intune-books-managedebook.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="561d7-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="561d7-116">Aktion zuweisen</span><span class="sxs-lookup"><span data-stu-id="561d7-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="561d7-117">Keine</span><span class="sxs-lookup"><span data-stu-id="561d7-117">None</span></span>|<span data-ttu-id="561d7-118">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="561d7-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="561d7-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="561d7-119">Properties</span></span>
|<span data-ttu-id="561d7-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="561d7-120">Property</span></span>|<span data-ttu-id="561d7-121">Typ</span><span class="sxs-lookup"><span data-stu-id="561d7-121">Type</span></span>|<span data-ttu-id="561d7-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="561d7-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="561d7-123">id</span><span class="sxs-lookup"><span data-stu-id="561d7-123">id</span></span>|<span data-ttu-id="561d7-124">string</span><span class="sxs-lookup"><span data-stu-id="561d7-124">String</span></span>|<span data-ttu-id="561d7-125">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="561d7-125">Key of the entity.</span></span>|
|<span data-ttu-id="561d7-126">displayName</span><span class="sxs-lookup"><span data-stu-id="561d7-126">displayName</span></span>|<span data-ttu-id="561d7-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="561d7-127">String</span></span>|<span data-ttu-id="561d7-128">Name des E-Books</span><span class="sxs-lookup"><span data-stu-id="561d7-128">Name of the eBook.</span></span>|
|<span data-ttu-id="561d7-129">description</span><span class="sxs-lookup"><span data-stu-id="561d7-129">description</span></span>|<span data-ttu-id="561d7-130">String</span><span class="sxs-lookup"><span data-stu-id="561d7-130">String</span></span>|<span data-ttu-id="561d7-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="561d7-131">Description.</span></span>|
|<span data-ttu-id="561d7-132">publisher</span><span class="sxs-lookup"><span data-stu-id="561d7-132">publisher</span></span>|<span data-ttu-id="561d7-133">String</span><span class="sxs-lookup"><span data-stu-id="561d7-133">String</span></span>|<span data-ttu-id="561d7-134">Herausgeber</span><span class="sxs-lookup"><span data-stu-id="561d7-134">Publisher.</span></span>|
|<span data-ttu-id="561d7-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="561d7-135">publishedDateTime</span></span>|<span data-ttu-id="561d7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="561d7-136">DateTimeOffset</span></span>|<span data-ttu-id="561d7-137">Datum und Uhrzeit der Veröffentlichung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="561d7-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="561d7-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="561d7-138">largeCover</span></span>|[<span data-ttu-id="561d7-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="561d7-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="561d7-140">Umschlagbild des Buchs</span><span class="sxs-lookup"><span data-stu-id="561d7-140">Book cover.</span></span>|
|<span data-ttu-id="561d7-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="561d7-141">createdDateTime</span></span>|<span data-ttu-id="561d7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="561d7-142">DateTimeOffset</span></span>|<span data-ttu-id="561d7-143">Datum und Uhrzeit der Erstellung der E-Book-Datei.</span><span class="sxs-lookup"><span data-stu-id="561d7-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="561d7-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="561d7-144">lastModifiedDateTime</span></span>|<span data-ttu-id="561d7-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="561d7-145">DateTimeOffset</span></span>|<span data-ttu-id="561d7-146">Datum und Uhrzeit der letzten Änderung des E-Books.</span><span class="sxs-lookup"><span data-stu-id="561d7-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="561d7-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="561d7-147">informationUrl</span></span>|<span data-ttu-id="561d7-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="561d7-148">String</span></span>|<span data-ttu-id="561d7-149">URL zur Seite mit weiteren Informationen.</span><span class="sxs-lookup"><span data-stu-id="561d7-149">The more information Url.</span></span>|
|<span data-ttu-id="561d7-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="561d7-150">privacyInformationUrl</span></span>|<span data-ttu-id="561d7-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="561d7-151">String</span></span>|<span data-ttu-id="561d7-152">URL zur Datenschutzerklärung</span><span class="sxs-lookup"><span data-stu-id="561d7-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="561d7-153">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="561d7-153">Relationships</span></span>
|<span data-ttu-id="561d7-154">Beziehung</span><span class="sxs-lookup"><span data-stu-id="561d7-154">Relationship</span></span>|<span data-ttu-id="561d7-155">Typ</span><span class="sxs-lookup"><span data-stu-id="561d7-155">Type</span></span>|<span data-ttu-id="561d7-156">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="561d7-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="561d7-157">assignments</span><span class="sxs-lookup"><span data-stu-id="561d7-157">assignments</span></span>|<span data-ttu-id="561d7-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="561d7-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="561d7-159">Die Liste der Zuweisungen für dieses E-Book.</span><span class="sxs-lookup"><span data-stu-id="561d7-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="561d7-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="561d7-160">installSummary</span></span>|[<span data-ttu-id="561d7-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="561d7-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="561d7-162">Die Installationszusammenfassung für die mobile App.</span><span class="sxs-lookup"><span data-stu-id="561d7-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="561d7-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="561d7-163">deviceStates</span></span>|<span data-ttu-id="561d7-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="561d7-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="561d7-165">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="561d7-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="561d7-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="561d7-166">userStateSummary</span></span>|<span data-ttu-id="561d7-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="561d7-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="561d7-168">Die Liste der Installationsstatus für das E-Book.</span><span class="sxs-lookup"><span data-stu-id="561d7-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="561d7-169">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="561d7-169">JSON Representation</span></span>
<span data-ttu-id="561d7-170">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="561d7-170">Here is a JSON representation of the resource.</span></span>
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



