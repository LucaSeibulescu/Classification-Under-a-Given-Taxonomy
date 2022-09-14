# Data Dictionary

## Item Hierarchy

Segment > Category > Class > Sub-Class > SKU

## Column Descriptions

| Column            | Description                                                                              |
| :---------------- | :--------------------------------------------------------------------------------------- |
| SKU               | The products stock keeping unit number.                                                  |
| ItemTitle         | The title of the product.                                                                |
| ItemDescription   | The description of the product.                                                          |
| ItemBulletPoint   | The bullet points description of the product.                                            |
| ItemDescription_2 | The description of the product.                                                          |
| Manufacturer      | The manufacturer name of the product.                                                    |
| MfrPartNum        | The manufacturer’s part number of the product.                                           |
| SellUOM           | The unit of measure (each/case/package).                                                 |
| ItemPrice         | The price of the product.                                                                |
| ItemFactTag       | Facts about the product.                                                                 |
| Segment           | The Segment code that the product belongs to in the hierarchical classification.         |
| Segment Name      | The Segment name that the product belongs to in the hierarchical classification.         |
| Category          | The category code that the product belongs to in the hierarchical classification.        |
| Category Name     | The name of the Category that the product belongs to in the hierarchical classification. |
| Class             | The class code that the product belongs to                                               |
| Class Name        | The name of the class that the product belongs to.                                       |
| Sub-Class         | The code of the Sub-Class that the product belongs to.                                   |
| Sub-Class Name    | The name of the Sub-Class that the product belongs to.                                   |

## Image Info

`image_info.txt` describes which images correspond to which products.
The `product` column indicates product `SKU`, the `image` column is a space-separated list of image names for this product.