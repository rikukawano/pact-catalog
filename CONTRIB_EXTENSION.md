<<<<<<< HEAD
# Contribute an Data Model Extension

To contribute a Data Model Extension, please follow these steps:

> **_NOTE:_** The following steps presuppose that you have already forked and cloned the `pact-catalog` repository. If that is not the case, please go back to the [main instructions](/README.md) and follow them in order.
=======
# Contribute an Industry Specific Extension

To contribute an Industry Specific Extension, please follow these steps:

> **_NOTE:_** The following steps pressupose that you have already forked and cloned the `pact-catalog` repository. If that is not the case, please go back to the [main instructions](/README.md) and follow them in order.
>>>>>>> 17ba26f88090995814bd5f25b231de1177ab0af8

### 1. Create a new extension path in the `data-model-extensions` directory

From the parent directory of your local repository run

```sh
<<<<<<< HEAD
mkdir -p catalog/data-model-extensions/@<your-user-id>/<extension-id>/<extension-version>
=======
mkdir -p catalog/data-model-extensions/@<your-name>/<extension-id>/<extension-version>
>>>>>>> 17ba26f88090995814bd5f25b231de1177ab0af8
```

### 2. Populate your extension's directory with the necessary files

From the parent directory of your local repository run

```sh
<<<<<<< HEAD
cd catalog/data-model-extensions/@<your-user-id>/<extension-id>/<extension-version>
=======
cd catalog/data-model-extensions/@<your-name>/<extension-id>/<extension-version>
>>>>>>> 17ba26f88090995814bd5f25b231de1177ab0af8
touch LICENSE && touch extension.json && touch schema.json && touch README.md
```

The `README.md` file is optional, but highly recommended. It should be filled with information about the extension and instructions on how to use it.

### 3. Fill in your extension's details

#### 3.1 `extension.json`

<<<<<<< HEAD
Open the `extension.json` file created in step 4. and fill it adapting the following structure:

<strong>Please note:</strong> All text between angle brackets (`< >`) should be replaced by actual values. Please make sure that the values replacing `<your-user-id>`, `<extension-id>` only include <strong>lowercase letters and dashes</strong> (instead of whitespace). The value replacing `<extension-version>` should follow the `X.Y.Z` format. Please make sure that these remain consistent. The value replacing `<MIT | CC0>` should be either `"MIT"` or `"CC0"`

```javascript
{
  "id": {
    "namespace": "@<your-user-id>", // e.g. 'ABC Institute' has user id "abc-institute" or "abc"
    "extension_name": "<extension-id>", // e.g. "example-extension"
    "version": "<extension-version>" // e.g. "0.0.0"
  },
  "name": "<Name of the extension>", // e.g. "Example Extension"
  "files": ["schema.json"],
  "author": {
    "name": "<Institution's name>", // e.g. "ABC Institute"
    "email": "<email>",
    "url": "<website>"
  },
  "license": "<MIT | CC0>", // select one
  "catalog_info": {
    "summary": "<Summary of the Extension>",
    "status": "draft",
    "authors": ["<your-user-id>"] // same as the one used in the `"namespace"` field (without '@')
=======
Open the `package.json` file created in step 4. and fill it adapting the following structure:

```json
{
  "id": {
    "namespace": "@<your-name>",
    "extension_name": "<extension-id>",
    "version": "<extension-version>"
  },
  "name": "<Name of the extension>",
  "files": ["schema.json"],
  "author": {
    "name": "<Institution's name>",
    "email": "<email>",
    "url": "<website>"
  },
  "license": "<license>",
  "catalog_info": {
    "summary": "<Summary of the Extension>",
    "status": "draft",
    "authors": ["<your-name>"]
>>>>>>> 17ba26f88090995814bd5f25b231de1177ab0af8
  },
  "industries": ["<industry>"]
}
```

<<<<<<< HEAD
Please refer to [this example](./catalog/data-model-extensions/@example-institution/example-extension/0.0.0/extension.json) to see how your `extension.json` should look like.


#### 3.2 `schema.json`

Open the `schema.json` file created in step 4. and fill it with your extension. This must be a valid [JSON schema](https://json-schema.org) based on [the Pathfinder Technical Specification V2](https://wbcsd.github.io/tr/2023/data-exchange-protocol-20230314/)
=======
Note: the value of `"license"` field must be either `"MIT"` or `"CC0"`.

#### 3.2 `schema.json`

Open the `schema.json` file created in step 4. and fill it with your extension. This must be a valid [JSON schema](https://json-schema.org) based on [the Pathfinder Technical Specification V2](https://pact-catalog-frontend.vercel.app/schemas/@wbcsd-product-footprint-2.0.0.schema.json)
>>>>>>> 17ba26f88090995814bd5f25b231de1177ab0af8

#### 3.3 `LICENSE`

Open the `LICENSE` file created in step 4. and fill it according to your license choice, which must be either `MIT` or `CC0`.

You can use [this template](https://github.com/sine-fdn/pact-catalog-frontend/blob/main/frontend/utils/MIT.txt) for the `MIT` license and copy [this text](https://github.com/sine-fdn/pact-catalog-frontend/blob/main/frontend/utils/CC0.txt) for the `CC0` license.

### 4. Commit your branch, push it, and open a Pull Request

<<<<<<< HEAD
Please continue from [step 6 of the main instructions](/README.md#4-commit-and-push-your-branch).


Your Pull Request will be reviewed and added to the PACT Online Catalog as soon as possible.

> **_NOTE:_** By submitting an Data Model Extension you acknowledge that you have read and accepted the [Terms and Conditions](/catalog/legal/TERMSANDCONDITIONS.md)
=======
Please continue from [step 4 of the main instructions](/README.md#4-commit-and-push-your-branch).

<strong>Please note:</strong> All text between angle brackets (`< >`) should be replaced by actual values. Please make sure that the values replacing `<your-name>`, `<extension-id>`, and `<extension-version>` remain consistent and that no whitespaces or special characters are used.

Your Pull Request will be reviewed and added to the PACT Online Catalog as soon as possible.

> **_NOTE:_** By submitting an Industry Specific Extension you acknowledge that you have read and accepted the [Terms and Conditions](/catalog/legal/TERMSANDCONDITIONS.md)
>>>>>>> 17ba26f88090995814bd5f25b231de1177ab0af8
