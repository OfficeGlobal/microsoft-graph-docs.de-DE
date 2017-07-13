<span data-ttu-id="31238-p105">In dieser Tabelle sind die möglichen Miniaturansichtgrößen definiert. Zwar können Sie jede beliebige Miniaturansichtgröße anfordern; bei den definierten Werten ist es jedoch wahrscheinlich, dass sie existieren und dass schnell ein Wert zurückgegeben wird:</span><span class="sxs-lookup"><span data-stu-id="31238-p105">This table defines the possible thumbnail sizes. While you can request any arbitrary thumbnail size, the defined values are likely to exist and return a value quickly:</span></span>

In dieser Tabelle sind die möglichen Miniaturansichtgrößen definiert. Zwar können Sie jede beliebige Miniaturansichtgröße anfordern; bei den definierten Werten ist es jedoch wahrscheinlich, dass sie existieren und dass schnell ein Wert zurückgegeben wird:

| <span data-ttu-id="31238-162">Name</span><span class="sxs-lookup"><span data-stu-id="31238-162">Name</span></span>           | <span data-ttu-id="31238-163">Auflösung</span><span class="sxs-lookup"><span data-stu-id="31238-163">Resolution</span></span>  | <span data-ttu-id="31238-164">Seitenverhältnis</span><span class="sxs-lookup"><span data-stu-id="31238-164">Aspect Ratio</span></span> | <span data-ttu-id="31238-165">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31238-165">Description</span></span>                                                          |
|:---------------|:------------|:-------------|:---------------------------------------------------------------------|
| `small`        | <span data-ttu-id="31238-166">96 longest
</span><span class="sxs-lookup"><span data-stu-id="31238-166">96 longest</span></span>  | <span data-ttu-id="31238-167">Original</span><span class="sxs-lookup"><span data-stu-id="31238-167">Original</span></span>     | <span data-ttu-id="31238-168">Kleine, stark komprimierte Miniaturansicht, zugeschnitten auf ein quadratisches Seitenverhältnis</span><span class="sxs-lookup"><span data-stu-id="31238-168">Small, highly compressed thumbnail cropped to a square aspect ratio.</span></span> |
| `medium`       | <span data-ttu-id="31238-169">176 longest</span><span class="sxs-lookup"><span data-stu-id="31238-169">176 longest</span></span> | <span data-ttu-id="31238-170">Original</span><span class="sxs-lookup"><span data-stu-id="31238-170">Original</span></span>     | <span data-ttu-id="31238-171">Zugeschnitten auf die standardmäßige Elementgröße für die OneDrive-Webansicht</span><span class="sxs-lookup"><span data-stu-id="31238-171">Cropped to the standard item size for the OneDrive web view.</span></span>         |
| `large`        | <span data-ttu-id="31238-172">800 longest
</span><span class="sxs-lookup"><span data-stu-id="31238-172">800 longest</span></span> | <span data-ttu-id="31238-173">Original</span><span class="sxs-lookup"><span data-stu-id="31238-173">Original</span></span>     | <span data-ttu-id="31238-174">Miniaturansicht, bei der die längste Kante auf 800 Pixel skaliert wurde</span><span class="sxs-lookup"><span data-stu-id="31238-174">Thumbnail with the longest edge resized to 800 pixels.</span></span>               |

## <span data-ttu-id="31238-175">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="31238-175">Remarks</span></span>
<a id="remarks" class="xliff"></a>

<span data-ttu-id="31238-176">**Hinweis:** Für OneDrive for Business und SharePoint gilt:</span><span class="sxs-lookup"><span data-stu-id="31238-176">**Note** In OneDrive for Business and SharePoint:</span></span>

* <span data-ttu-id="31238-177">Die folgenden Aufrufe können nicht zur Erweiterung der Miniaturansichtsammlung verwendet werden: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span><span class="sxs-lookup"><span data-stu-id="31238-177">Using these calls to expand the thumbnails collection will not work: `GET /drive/root:/{item-path}?expand=children(expand=thumbnails)`
  `GET /drive/items/{item-id}/children?expand=thumbnails`</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata and content for thumbnails of multiple sizes for OneDrive items.",
  "keywords": "thumbnail,content,download,sizes",
  "section": "documentation",
  "tocPath": "OneDrive/Item/List thumbnails"
} -->
