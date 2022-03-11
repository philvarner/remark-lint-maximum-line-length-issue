# Table


This line is simply not toooooooooooooooooooooooooooooooooooooooooooo
long.

This is also fine: <http://this-long-url-with-a-long-domain.co.uk/a-long-path?query=variables>

<http://this-link-is-fine.com>

`alphaBravoCharlieDeltaEchoFoxtrotGolfHotelIndiaJuliettKiloLimaMikeNovemberOscarPapaQuebec.romeo()`

[foo](http://this-long-url-with-a-long-domain-is-ok.co.uk/a-long-path?query=variables)

<http://this-long-url-with-a-long-domain-is-ok.co.uk/a-long-path?query=variables>

![foo](http://this-long-url-with-a-long-domain-is-ok.co.uk/a-long-path?query=variables)

| An | exception | is | line | length | in | long | tables | because | those | can’t | just |
| -- | --------- | -- | ---- | ------ | -- | ---- | ------ | ------- | ----- | ----- | ---- |
| be | helped    |    |      |        |    |      |        |         |       |       | .    |

<a><b><i><p><q><s><u>alpha bravo charlie delta echo foxtrot golf</u></s></q></p></i></b></a>

The following is also fine (note the `.`), because there is no whitespace.

<http://this-long-url-with-a-long-domain-is-ok.co.uk/a-long-path?query=variables>.

In addition, definitions are also fine:

[foo]: <http://this-long-url-with-a-long-domain-is-ok.co.uk/a-long-path?query=variables>



| Endpoint                                            | Specified in               | Link Relationship | Returns                                                                                             | Description                                                                                                                                |
| --------------------------------------------------- | -------------------------- | ----------------- | --------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| `/`                                                 | [Core](core)               | root              | [Catalog](stac-spec/catalog-spec/catalog-spec.md)                                                   | Extends `/` from OAFeat to return a full STAC catalog.                                                                                     |
| `/search`                                           | [Item Search](item-search) | search            | [ItemCollection](fragments/itemcollection/README.md)                                                | Retrieves a group of Item objects matching the provided search predicates, probably containing search metadata from the `search` extension |
| **`/collections`**                                  | [OAFeat](ogcapi-features)  | data              | JSON                                                                                                | Object with a list of Collection objects contained in the catalog and links                                                                |
| **`/conformance`**                                  | [OAFeat](ogcapi-features)  | conformance       | JSON                                                                                                | Info about standards to which the API conforms                                                                                             |
| `/api`                                              | [OAFeat](ogcapi-features)  | service-desc      | any                                                                           | The description of the endpoints in this service                                                                                    |
| **`/collections/{collectionId}`**                   | [OAFeat](ogcapi-features)  | collection        | Collection                                                                                          | Returns single Collection JSON                                                                                                             |
| **`/collections/{collectionId}/items`**             | [OAFeat](ogcapi-features)  | items             | ItemCollection                                                                                      | GeoJSON FeatureCollection-conformant entity of Item objects in collection                                                                  |
| **`/collections/{collectionId}/items/{featureId}`** | [OAFeat](ogcapi-features)  | item              | Returns single Item (GeoJSON Feature). This relation is usually not used in OAFeat implementations. |
