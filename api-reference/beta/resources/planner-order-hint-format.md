---
title: Verwenden von ORDER-Hinweisen in Planner
description: '`)'
author: TarkanSevilmis
localization_priority: Normal
ms.openlocfilehash: d7e4af4928d996bf810245b011e22baade37a431
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891959"
---
# <a name="using-order-hints-in-planner"></a><span data-ttu-id="95e1a-103">Verwenden von ORDER-Hinweisen in Planner</span><span class="sxs-lookup"><span data-stu-id="95e1a-103">Using order hints in Planner</span></span>

> <span data-ttu-id="95e1a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="95e1a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95e1a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="95e1a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95e1a-p102">Objekte in Planner identifizieren ihre Sortierreihenfolge anhand von ORDER-Hinweisen. Die Werte von ORDER-Hinweisen sind Zeichenfolgen. Die Clients können die Zeichenfolgen basierend auf dem Ordnungswert von darin enthaltenen Zeichen sortieren, um die Reihenfolge von Elementen zu identifizieren. Die Zeichen werden ab dem Anfang der Zeichenfolge verglichen, bis ein Unterschied in den Ordnungswerten der Zeichen gefunden wird oder bis eine Zeichenfolge endet. In diesem Fall wird die kürzere Zeichenfolge vor der längeren sortiert. Die Werte können beliebige Zeichen zwischen den Ordnungszahlen 32 (Leerzeichen) und 126 enthalten (`~`).</span><span class="sxs-lookup"><span data-stu-id="95e1a-p102">Objects in Planner identify their sort order by order hints. The order hint values are strings. The clients can sort the strings based on ordinal value of characters in them to identify the order of items. The characters are compared from the beginning of the string, until a difference is encountered in the ordinal values of characters, or one string ends, in which case the shorter string would be sorted before the longer. The values can contain any character between ordinals 32 (space) and 126 (`~`)</span></span>

<span data-ttu-id="95e1a-p103">Als Beispiel würde ein Element mit dem ORDER-Hinweis `a` (Ordnungswert 97) vor einem anderen Element mit dem ORDER-Hinweis `z` (Ordnungswert 122) platziert werden. Ein Element mit dem ORDER-Hinweis `abc` (Ordnungswerte 97, 98, 99) würde vor einem anderen Element mit dem ORDER-Hinweis `abd` (Ordnungswerte 97, 98, 100) platziert werden. Ein Element mit dem ORDER-Hinweis `a` würde vor einem anderen Element mit dem ORDER-Hinweis `ab` platziert, da alle vorhandenen Zeichen identisch sind und `a` kürzer ist.</span><span class="sxs-lookup"><span data-stu-id="95e1a-p103">As an example, an item with order hint `a` (ordinal value 97) would be placed before another item with order hint `z` (ordinal value 122). An item with order hint `abc` (ordinal values 97, 98, 99), would be placed before another item with order hint `abd` (ordinal values 97, 98, 100). An item with order hint `a` would be placed before another item with order hint `ab` since all existing characters are the same, and `a` is shorter.</span></span>

<span data-ttu-id="95e1a-p104">Die Werte für alle ORDER-Hinweise werden vom Dienst berechnet. Der Client kann die Reihenfolge von Elementen ändern, indem der ORDER-Hinweis für das Element angegeben wird, das zwischen zwei Elementen verschoben wurde, indem der ORDER-Hinweis auf den folgenden Wert festgelegt wird: `<previous order hint> <next order hint>!`, wobei `<previous order hint>` durch den ORDER-Hinweis des Elements ersetzt werden muss, das sich vor der neuen gewünschten Position befindet, und `<next order hint>` durch den ORDER-Hinweis des Elements ersetzt werden muss, das sich nach der neuen gewünschten Position befindet. Es gibt ein Leerzeichen zwischen den Werten dieser ORDER-Hinweise, und `!` wird an den gesamten Wert angehängt. Wenn eines der Elemente nicht vorhanden ist, sollte stattdessen eine leere Zeichenfolge verwendet werden. Dieser Wert kann auch aus vorherigen Berechnungen zusammengestellt werden, und kann im Client verwendet werden, um Elemente genau wie vom Dienst zurückgegebene ORDER-Hinweise zu sortieren. Nachdem der Client diese Werte an eine Aktualisierung gesendet hat, berechnet der Dienst einen kurzen Wert, der an der gewünschten Position sortiert wird.</span><span class="sxs-lookup"><span data-stu-id="95e1a-p104">The values for all order hints are calculated by the service. The client can reorder items by specifying the order hint for the item that got moved between two items with by setting the order hint to the following value: `<previous order hint> <next order hint>!`, where `<previous order hint>` is to be replaced by the order hint of the item that comes before the new desired location, and `<next order hint>` is to be replaced by the order hint of the item that comes after the new desired location. There is a space character between these order hint values, and the entire value is suffixed with `!`. If either item isn't present, empty string should be used instead. This value can also be composed of previous calculations, and can be used in the client to sort items exactly like service returned order hints. Once the client sends these values in an update, the service will calculate a short value that sorts in the desired location.</span></span>

> <span data-ttu-id="95e1a-120">**Hinweis:** In den folgenden Beispielen werden die tatsächliche Reihenfolge Hint Werte in einfache Anführungszeichen umgeben (`'`) aus Gründen der Übersichtlichkeit jedoch diese sind nicht Teil der Daten und müssen nicht mit dem Dienst gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="95e1a-120">**Note:** In the following examples, the actual order hint values are surrounded in single quote characters (`'`) for clarity, however these are not part of the data, and must not be sent to the service.</span></span>
 
<span data-ttu-id="95e1a-121">Sehen Sie sich als Beispiel die folgende Liste sortierter ORDER-Hinweise an:</span><span class="sxs-lookup"><span data-stu-id="95e1a-121">As an example, consider the following list of sorted order hints:</span></span>

1. <span data-ttu-id="95e1a-122">Element 1 (ORDER-Hinweis: `'5637'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-122">Item 1 (Order Hint: `'5637'`)</span></span>
2. <span data-ttu-id="95e1a-123">Element 2 (ORDER-Hinweis: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-123">Item 2 (Order Hint: `'adhg'`)</span></span>

<span data-ttu-id="95e1a-124">Durch Platzieren eines Elements 3 vor Element 1, anschließendes Platzieren von Element 4 zwischen Element 1 und Element 2 und anschließendes Platzieren von Element 5 nach Element 2 würden die folgenden ORDER-Hinweise auf dem Client erstellt.</span><span class="sxs-lookup"><span data-stu-id="95e1a-124">Placing an Item 3 before Item 1, then placing item 4 between Item 1 and Item 2, and then placing item 5 after Item 2, would create the following order hints on the client.</span></span> 

1. <span data-ttu-id="95e1a-125">Element 3 (ORDER-Hinweis: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-125">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="95e1a-126">Element 1 (ORDER-Hinweis: `'5637'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-126">Item 1 (Order Hint: `'5637'`)</span></span>
3. <span data-ttu-id="95e1a-127">Element 4 (ORDER-Hinweis: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-127">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="95e1a-128">Element 2 (ORDER-Hinweis: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-128">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="95e1a-129">Element 5 (ORDER-Hinweis: `'adhg !'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-129">Item 5 (Order Hint: `'adhg !'`)</span></span>

<span data-ttu-id="95e1a-130">Durch Verschieben von Element 1 an das Ende der Liste würde Folgendes generiert:</span><span class="sxs-lookup"><span data-stu-id="95e1a-130">Then, moving item 1 to the end of the list would generate:</span></span>

1. <span data-ttu-id="95e1a-131">Element 3 (ORDER-Hinweis: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-131">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="95e1a-132">Element 4 (ORDER-Hinweis: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-132">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
3. <span data-ttu-id="95e1a-133">Element 2 (ORDER-Hinweis: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-133">Item 2 (Order Hint: `'adhg'`)</span></span>
4. <span data-ttu-id="95e1a-134">Element 5 (ORDER-Hinweis: `'adhg !'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-134">Item 5 (Order Hint: `'adhg !'`)</span></span>
5. <span data-ttu-id="95e1a-135">Element 1 (ORDER-Hinweis: `'adhg ! !'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-135">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="95e1a-136">Durch Verschieben von Element 5 zwischen Element 3 und Element 4 würde schließlich Folgendes generiert:</span><span class="sxs-lookup"><span data-stu-id="95e1a-136">Finally moving Item 5 between Item 3 and Item 4 would generate:</span></span>

1. <span data-ttu-id="95e1a-137">Element 3 (ORDER-Hinweis: `' 5637!'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-137">Item 3 (Order Hint: `' 5637!'`)</span></span>
2. <span data-ttu-id="95e1a-138">Element 5 (ORDER-Hinweis: `' 5637! 5637 adhg!!'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-138">Item 5 (Order Hint: `' 5637! 5637 adhg!!'`)</span></span>
3. <span data-ttu-id="95e1a-139">Element 4 (ORDER-Hinweis: `'5637 adhg!'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-139">Item 4 (Order Hint: `'5637 adhg!'`)</span></span>
4. <span data-ttu-id="95e1a-140">Element 2 (ORDER-Hinweis: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-140">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="95e1a-141">Element 1 (ORDER-Hinweis: `'adhg ! !'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-141">Item 1 (Order Hint: `'adhg ! !'`)</span></span>

<span data-ttu-id="95e1a-142">Wenn diese Änderungen auf Reihenfolge Hint Werte an den Dienst in Patch Anfragen gesendet werden, wird der Dienst geeignete Werte berechnen, die die Reihenfolge für die direkte Verwendung durch den Client beibehalten.</span><span class="sxs-lookup"><span data-stu-id="95e1a-142">When these changes to order hint values are sent to the service in patch requests, the service will calculate proper values that keep the order intended by the client.</span></span> <span data-ttu-id="95e1a-143">Der Client kann die direkte If Werte erhalten die `Prefer: return=representation` Einstellung Kopfzeile wird angegeben, der `PATCH` Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="95e1a-143">The client can obtain the values immediate if the `Prefer: return=representation` preference header is specified in the `PATCH` requests.</span></span> <span data-ttu-id="95e1a-144">Die Werte für die oben genannten Fall sehen in etwa wie folgt aus (die tatsächlichen Werte können anders lauten).</span><span class="sxs-lookup"><span data-stu-id="95e1a-144">The values for the case above may look like the following (the actual values may differ).</span></span> 

1. <span data-ttu-id="95e1a-145">Element 3 (ORDER-Hinweis: `'432b'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-145">Item 3 (Order Hint: `'432b'`)</span></span>
2. <span data-ttu-id="95e1a-146">Element 5 (ORDER-Hinweis: `'6F"#'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-146">Item 5 (Order Hint: `'6F"#'`)</span></span>
3. <span data-ttu-id="95e1a-147">Element 4 (ORDER-Hinweis: `'7A$6'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-147">Item 4 (Order Hint: `'7A$6'`)</span></span>
4. <span data-ttu-id="95e1a-148">Element 2 (ORDER-Hinweis: `'adhg'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-148">Item 2 (Order Hint: `'adhg'`)</span></span>
5. <span data-ttu-id="95e1a-149">Element 1 (ORDER-Hinweis: `'de5%'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-149">Item 1 (Order Hint: `'de5%'`)</span></span>

<span data-ttu-id="95e1a-p106">ORDER-Hinweise können für das Erstellen des ersten Elements in der Liste als ` !` angegeben werden, da in diesem Fall weder ein vorheriges noch ein nächstes Element vorhanden ist, dies ist jedoch nicht erforderlich, da der Dienst Werte für alle ORDER-Hinweise für Elemente automatisch generiert, wenn diese während der Erstellung des Elements nicht angegeben werden. Im folgenden Beispiel werden die ORDER-Hinweise veranschaulicht, die verwendet werden sollten, wenn Element in einer zuvor leeren Liste platziert werden. Fügen Sie das erste Element hinzu:</span><span class="sxs-lookup"><span data-stu-id="95e1a-p106">Order Hints can be specified for creating the first item in the list as ` !`, since neither a previous or a next item exists in that case, however this is unnecessary, as the service will auto-generate values for all order hint values on items if they are not specified during creation of the item. Following example illustrates the order hints should be used when placing items in a previously empty list. Add the first item:</span></span>

1. <span data-ttu-id="95e1a-153">Element 1 (ORDER-Hinweis: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-153">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="95e1a-154">Fügen Sie das zweite Elemente am Anfang hinzu:</span><span class="sxs-lookup"><span data-stu-id="95e1a-154">Add the second item to top:</span></span>

1. <span data-ttu-id="95e1a-155">Element 2 (ORDER-Hinweis: `'  !!'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-155">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="95e1a-156">Element 1 (ORDER-Hinweis: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-156">Item 1 (Order Hint: `' !'`)</span></span>

<span data-ttu-id="95e1a-157">Fügen Sie das dritte Element am Ende hinzu:</span><span class="sxs-lookup"><span data-stu-id="95e1a-157">Add the third item to bottom:</span></span>

1. <span data-ttu-id="95e1a-158">Element 2 (ORDER-Hinweis: `'  !!'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-158">Item 2 (Order Hint: `'  !!'`)</span></span>
2. <span data-ttu-id="95e1a-159">Element 1 (ORDER-Hinweis: `' !'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-159">Item 1 (Order Hint: `' !'`)</span></span>
3. <span data-ttu-id="95e1a-160">Element 3 (ORDER-Hinweis: `' ! !'`)</span><span class="sxs-lookup"><span data-stu-id="95e1a-160">Item 3 (Order Hint: `' ! !'`)</span></span>







