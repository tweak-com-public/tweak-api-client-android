# tweak-api

## Requirements

Building the API client library requires [Maven](https://maven.apache.org/) to be installed.

## Installation

To install the API client library to your local Maven repository, simply execute:

```shell
mvn install
```

To deploy it to a remote Maven repository instead, configure the settings of the repository and execute:

```shell
mvn deploy
```

Refer to the [official documentation](https://maven.apache.org/plugins/maven-deploy-plugin/usage.html) for more information.

### Maven users

Add this dependency to your project's POM:

```xml
<dependency>
    <groupId>com.tweak</groupId>
    <artifactId>tweak-api</artifactId>
    <version>1.0.0</version>
    <scope>compile</scope>
</dependency>
```

### Gradle users

Add this dependency to your project's build file:

```groovy
compile "com.tweak:tweak-api:1.0.0"
```

### Others

At first generate the JAR by executing:

    mvn package

Then manually install the following JARs:

* target/tweak-api-1.0.0.jar
* target/lib/*.jar

## Getting Started

Please follow the [installation](#installation) instruction and execute the following Java code:

```java

import com.tweak.api.CategoryApi;

public class CategoryApiExample {

    public static void main(String[] args) {
        CategoryApi apiInstance = new CategoryApi();
        String where = "where_example"; // String | Criteria to match model instances
        try {
            InlineResponse200 result = apiInstance.categoryCount(where);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling CategoryApi#categoryCount");
            e.printStackTrace();
        }
    }
}

```

## Documentation for API Endpoints

All URIs are relative to *https://apidevcdn.tweak.com/api*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*CategoryApi* | [**categoryCount**](docs/CategoryApi.md#categoryCount) | **GET** /Categories/count | Count instances of the model matched by where from the data source.
*CategoryApi* | [**categoryCreate**](docs/CategoryApi.md#categoryCreate) | **POST** /Categories | Create a new instance of the model and persist it into the data source.
*CategoryApi* | [**categoryCreateChangeStreamGetCategoriesChangeStream**](docs/CategoryApi.md#categoryCreateChangeStreamGetCategoriesChangeStream) | **GET** /Categories/change-stream | Create a change stream.
*CategoryApi* | [**categoryCreateChangeStreamPostCategoriesChangeStream**](docs/CategoryApi.md#categoryCreateChangeStreamPostCategoriesChangeStream) | **POST** /Categories/change-stream | Create a change stream.
*CategoryApi* | [**categoryDeleteById**](docs/CategoryApi.md#categoryDeleteById) | **DELETE** /Categories/{id} | Delete a model instance by {{id}} from the data source.
*CategoryApi* | [**categoryExistsGetCategoriesidExists**](docs/CategoryApi.md#categoryExistsGetCategoriesidExists) | **GET** /Categories/{id}/exists | Check whether a model instance exists in the data source.
*CategoryApi* | [**categoryExistsHeadCategoriesid**](docs/CategoryApi.md#categoryExistsHeadCategoriesid) | **HEAD** /Categories/{id} | Check whether a model instance exists in the data source.
*CategoryApi* | [**categoryFind**](docs/CategoryApi.md#categoryFind) | **GET** /Categories | Find all instances of the model matched by filter from the data source.
*CategoryApi* | [**categoryFindById**](docs/CategoryApi.md#categoryFindById) | **GET** /Categories/{id} | Find a model instance by {{id}} from the data source.
*CategoryApi* | [**categoryFindOne**](docs/CategoryApi.md#categoryFindOne) | **GET** /Categories/findOne | Find first instance of the model matched by filter from the data source.
*CategoryApi* | [**categoryPrototypeCountChildren**](docs/CategoryApi.md#categoryPrototypeCountChildren) | **GET** /Categories/{id}/children/count | Counts children of Category.
*CategoryApi* | [**categoryPrototypeCreateChildren**](docs/CategoryApi.md#categoryPrototypeCreateChildren) | **POST** /Categories/{id}/children | Creates a new instance in children of this model.
*CategoryApi* | [**categoryPrototypeDeleteChildren**](docs/CategoryApi.md#categoryPrototypeDeleteChildren) | **DELETE** /Categories/{id}/children | Deletes all children of this model.
*CategoryApi* | [**categoryPrototypeDestroyByIdChildren**](docs/CategoryApi.md#categoryPrototypeDestroyByIdChildren) | **DELETE** /Categories/{id}/children/{fk} | Delete a related item by id for children.
*CategoryApi* | [**categoryPrototypeFindByIdChildren**](docs/CategoryApi.md#categoryPrototypeFindByIdChildren) | **GET** /Categories/{id}/children/{fk} | Find a related item by id for children.
*CategoryApi* | [**categoryPrototypeGetChildren**](docs/CategoryApi.md#categoryPrototypeGetChildren) | **GET** /Categories/{id}/children | Queries children of Category.
*CategoryApi* | [**categoryPrototypeGetParent**](docs/CategoryApi.md#categoryPrototypeGetParent) | **GET** /Categories/{id}/parent | Fetches belongsTo relation parent.
*CategoryApi* | [**categoryPrototypeUpdateAttributesPatchCategoriesid**](docs/CategoryApi.md#categoryPrototypeUpdateAttributesPatchCategoriesid) | **PATCH** /Categories/{id} | Patch attributes for a model instance and persist it into the data source.
*CategoryApi* | [**categoryPrototypeUpdateAttributesPutCategoriesid**](docs/CategoryApi.md#categoryPrototypeUpdateAttributesPutCategoriesid) | **PUT** /Categories/{id} | Patch attributes for a model instance and persist it into the data source.
*CategoryApi* | [**categoryPrototypeUpdateByIdChildren**](docs/CategoryApi.md#categoryPrototypeUpdateByIdChildren) | **PUT** /Categories/{id}/children/{fk} | Update a related item by id for children.
*CategoryApi* | [**categoryReplaceById**](docs/CategoryApi.md#categoryReplaceById) | **POST** /Categories/{id}/replace | Replace attributes for a model instance and persist it into the data source.
*CategoryApi* | [**categoryReplaceOrCreate**](docs/CategoryApi.md#categoryReplaceOrCreate) | **POST** /Categories/replaceOrCreate | Replace an existing model instance or insert a new one into the data source.
*CategoryApi* | [**categoryUpdateAll**](docs/CategoryApi.md#categoryUpdateAll) | **POST** /Categories/update | Update instances of the model matched by {{where}} from the data source.
*CategoryApi* | [**categoryUpsertPatchCategories**](docs/CategoryApi.md#categoryUpsertPatchCategories) | **PATCH** /Categories | Patch an existing model instance or insert a new one into the data source.
*CategoryApi* | [**categoryUpsertPutCategories**](docs/CategoryApi.md#categoryUpsertPutCategories) | **PUT** /Categories | Patch an existing model instance or insert a new one into the data source.
*CategoryApi* | [**categoryUpsertWithWhere**](docs/CategoryApi.md#categoryUpsertWithWhere) | **POST** /Categories/upsertWithWhere | Update an existing model instance or insert a new one into the data source based on the where criteria.
*CustomerApi* | [**customerConfirm**](docs/CustomerApi.md#customerConfirm) | **GET** /Customers/confirm | Confirm a user registration with email verification token.
*CustomerApi* | [**customerCount**](docs/CustomerApi.md#customerCount) | **GET** /Customers/count | Count instances of the model matched by where from the data source.
*CustomerApi* | [**customerCreate**](docs/CustomerApi.md#customerCreate) | **POST** /Customers | Create a new instance of the model and persist it into the data source.
*CustomerApi* | [**customerCreateChangeStreamGetCustomersChangeStream**](docs/CustomerApi.md#customerCreateChangeStreamGetCustomersChangeStream) | **GET** /Customers/change-stream | Create a change stream.
*CustomerApi* | [**customerCreateChangeStreamPostCustomersChangeStream**](docs/CustomerApi.md#customerCreateChangeStreamPostCustomersChangeStream) | **POST** /Customers/change-stream | Create a change stream.
*CustomerApi* | [**customerDeleteById**](docs/CustomerApi.md#customerDeleteById) | **DELETE** /Customers/{id} | Delete a model instance by {{id}} from the data source.
*CustomerApi* | [**customerExistsGetCustomersidExists**](docs/CustomerApi.md#customerExistsGetCustomersidExists) | **GET** /Customers/{id}/exists | Check whether a model instance exists in the data source.
*CustomerApi* | [**customerExistsHeadCustomersid**](docs/CustomerApi.md#customerExistsHeadCustomersid) | **HEAD** /Customers/{id} | Check whether a model instance exists in the data source.
*CustomerApi* | [**customerFind**](docs/CustomerApi.md#customerFind) | **GET** /Customers | Find all instances of the model matched by filter from the data source.
*CustomerApi* | [**customerFindById**](docs/CustomerApi.md#customerFindById) | **GET** /Customers/{id} | Find a model instance by {{id}} from the data source.
*CustomerApi* | [**customerFindOne**](docs/CustomerApi.md#customerFindOne) | **GET** /Customers/findOne | Find first instance of the model matched by filter from the data source.
*CustomerApi* | [**customerLogin**](docs/CustomerApi.md#customerLogin) | **POST** /Customers/login | Login a user with username/email and password.
*CustomerApi* | [**customerLogout**](docs/CustomerApi.md#customerLogout) | **POST** /Customers/logout | Logout a user with access token.
*CustomerApi* | [**customerPrototypeCountAccessTokens**](docs/CustomerApi.md#customerPrototypeCountAccessTokens) | **GET** /Customers/{id}/accessTokens/count | Counts accessTokens of Customer.
*CustomerApi* | [**customerPrototypeCountDesigns**](docs/CustomerApi.md#customerPrototypeCountDesigns) | **GET** /Customers/{id}/designs/count | Counts designs of Customer.
*CustomerApi* | [**customerPrototypeCreateAccessTokens**](docs/CustomerApi.md#customerPrototypeCreateAccessTokens) | **POST** /Customers/{id}/accessTokens | Creates a new instance in accessTokens of this model.
*CustomerApi* | [**customerPrototypeCreateDesigns**](docs/CustomerApi.md#customerPrototypeCreateDesigns) | **POST** /Customers/{id}/designs | Creates a new instance in designs of this model.
*CustomerApi* | [**customerPrototypeDeleteAccessTokens**](docs/CustomerApi.md#customerPrototypeDeleteAccessTokens) | **DELETE** /Customers/{id}/accessTokens | Deletes all accessTokens of this model.
*CustomerApi* | [**customerPrototypeDeleteDesigns**](docs/CustomerApi.md#customerPrototypeDeleteDesigns) | **DELETE** /Customers/{id}/designs | Deletes all designs of this model.
*CustomerApi* | [**customerPrototypeDestroyByIdAccessTokens**](docs/CustomerApi.md#customerPrototypeDestroyByIdAccessTokens) | **DELETE** /Customers/{id}/accessTokens/{fk} | Delete a related item by id for accessTokens.
*CustomerApi* | [**customerPrototypeDestroyByIdDesigns**](docs/CustomerApi.md#customerPrototypeDestroyByIdDesigns) | **DELETE** /Customers/{id}/designs/{fk} | Delete a related item by id for designs.
*CustomerApi* | [**customerPrototypeFindByIdAccessTokens**](docs/CustomerApi.md#customerPrototypeFindByIdAccessTokens) | **GET** /Customers/{id}/accessTokens/{fk} | Find a related item by id for accessTokens.
*CustomerApi* | [**customerPrototypeFindByIdDesigns**](docs/CustomerApi.md#customerPrototypeFindByIdDesigns) | **GET** /Customers/{id}/designs/{fk} | Find a related item by id for designs.
*CustomerApi* | [**customerPrototypeGetAccessTokens**](docs/CustomerApi.md#customerPrototypeGetAccessTokens) | **GET** /Customers/{id}/accessTokens | Queries accessTokens of Customer.
*CustomerApi* | [**customerPrototypeGetDesigns**](docs/CustomerApi.md#customerPrototypeGetDesigns) | **GET** /Customers/{id}/designs | Queries designs of Customer.
*CustomerApi* | [**customerPrototypeUpdateAttributesPatchCustomersid**](docs/CustomerApi.md#customerPrototypeUpdateAttributesPatchCustomersid) | **PATCH** /Customers/{id} | Patch attributes for a model instance and persist it into the data source.
*CustomerApi* | [**customerPrototypeUpdateAttributesPutCustomersid**](docs/CustomerApi.md#customerPrototypeUpdateAttributesPutCustomersid) | **PUT** /Customers/{id} | Patch attributes for a model instance and persist it into the data source.
*CustomerApi* | [**customerPrototypeUpdateByIdAccessTokens**](docs/CustomerApi.md#customerPrototypeUpdateByIdAccessTokens) | **PUT** /Customers/{id}/accessTokens/{fk} | Update a related item by id for accessTokens.
*CustomerApi* | [**customerPrototypeUpdateByIdDesigns**](docs/CustomerApi.md#customerPrototypeUpdateByIdDesigns) | **PUT** /Customers/{id}/designs/{fk} | Update a related item by id for designs.
*CustomerApi* | [**customerReplaceById**](docs/CustomerApi.md#customerReplaceById) | **POST** /Customers/{id}/replace | Replace attributes for a model instance and persist it into the data source.
*CustomerApi* | [**customerReplaceOrCreate**](docs/CustomerApi.md#customerReplaceOrCreate) | **POST** /Customers/replaceOrCreate | Replace an existing model instance or insert a new one into the data source.
*CustomerApi* | [**customerResetPassword**](docs/CustomerApi.md#customerResetPassword) | **POST** /Customers/reset | Reset password for a user with email.
*CustomerApi* | [**customerUpdateAll**](docs/CustomerApi.md#customerUpdateAll) | **POST** /Customers/update | Update instances of the model matched by {{where}} from the data source.
*CustomerApi* | [**customerUpsertPatchCustomers**](docs/CustomerApi.md#customerUpsertPatchCustomers) | **PATCH** /Customers | Patch an existing model instance or insert a new one into the data source.
*CustomerApi* | [**customerUpsertPutCustomers**](docs/CustomerApi.md#customerUpsertPutCustomers) | **PUT** /Customers | Patch an existing model instance or insert a new one into the data source.
*CustomerApi* | [**customerUpsertWithWhere**](docs/CustomerApi.md#customerUpsertWithWhere) | **POST** /Customers/upsertWithWhere | Update an existing model instance or insert a new one into the data source based on the where criteria.
*DesignApi* | [**designCount**](docs/DesignApi.md#designCount) | **GET** /Designs/count | Count instances of the model matched by where from the data source.
*DesignApi* | [**designCreate**](docs/DesignApi.md#designCreate) | **POST** /Designs | Create a new instance of the model and persist it into the data source.
*DesignApi* | [**designCreateChangeStreamGetDesignsChangeStream**](docs/DesignApi.md#designCreateChangeStreamGetDesignsChangeStream) | **GET** /Designs/change-stream | Create a change stream.
*DesignApi* | [**designCreateChangeStreamPostDesignsChangeStream**](docs/DesignApi.md#designCreateChangeStreamPostDesignsChangeStream) | **POST** /Designs/change-stream | Create a change stream.
*DesignApi* | [**designDeleteById**](docs/DesignApi.md#designDeleteById) | **DELETE** /Designs/{id} | Delete a model instance by {{id}} from the data source.
*DesignApi* | [**designExistsGetDesignsidExists**](docs/DesignApi.md#designExistsGetDesignsidExists) | **GET** /Designs/{id}/exists | Check whether a model instance exists in the data source.
*DesignApi* | [**designExistsHeadDesignsid**](docs/DesignApi.md#designExistsHeadDesignsid) | **HEAD** /Designs/{id} | Check whether a model instance exists in the data source.
*DesignApi* | [**designFind**](docs/DesignApi.md#designFind) | **GET** /Designs | Find all instances of the model matched by filter from the data source.
*DesignApi* | [**designFindById**](docs/DesignApi.md#designFindById) | **GET** /Designs/{id} | Find a model instance by {{id}} from the data source.
*DesignApi* | [**designFindOne**](docs/DesignApi.md#designFindOne) | **GET** /Designs/findOne | Find first instance of the model matched by filter from the data source.
*DesignApi* | [**designPrototypeCountCategories**](docs/DesignApi.md#designPrototypeCountCategories) | **GET** /Designs/{id}/categories/count | Counts categories of Design.
*DesignApi* | [**designPrototypeCountTags**](docs/DesignApi.md#designPrototypeCountTags) | **GET** /Designs/{id}/tags/count | Counts tags of Design.
*DesignApi* | [**designPrototypeCreateCategories**](docs/DesignApi.md#designPrototypeCreateCategories) | **POST** /Designs/{id}/categories | Creates a new instance in categories of this model.
*DesignApi* | [**designPrototypeCreateTags**](docs/DesignApi.md#designPrototypeCreateTags) | **POST** /Designs/{id}/tags | Creates a new instance in tags of this model.
*DesignApi* | [**designPrototypeDeleteCategories**](docs/DesignApi.md#designPrototypeDeleteCategories) | **DELETE** /Designs/{id}/categories | Deletes all categories of this model.
*DesignApi* | [**designPrototypeDeleteTags**](docs/DesignApi.md#designPrototypeDeleteTags) | **DELETE** /Designs/{id}/tags | Deletes all tags of this model.
*DesignApi* | [**designPrototypeDestroyByIdCategories**](docs/DesignApi.md#designPrototypeDestroyByIdCategories) | **DELETE** /Designs/{id}/categories/{fk} | Delete a related item by id for categories.
*DesignApi* | [**designPrototypeDestroyByIdTags**](docs/DesignApi.md#designPrototypeDestroyByIdTags) | **DELETE** /Designs/{id}/tags/{fk} | Delete a related item by id for tags.
*DesignApi* | [**designPrototypeFindByIdCategories**](docs/DesignApi.md#designPrototypeFindByIdCategories) | **GET** /Designs/{id}/categories/{fk} | Find a related item by id for categories.
*DesignApi* | [**designPrototypeFindByIdTags**](docs/DesignApi.md#designPrototypeFindByIdTags) | **GET** /Designs/{id}/tags/{fk} | Find a related item by id for tags.
*DesignApi* | [**designPrototypeGetCategories**](docs/DesignApi.md#designPrototypeGetCategories) | **GET** /Designs/{id}/categories | Queries categories of Design.
*DesignApi* | [**designPrototypeGetCustomer**](docs/DesignApi.md#designPrototypeGetCustomer) | **GET** /Designs/{id}/customer | Fetches belongsTo relation customer.
*DesignApi* | [**designPrototypeGetTags**](docs/DesignApi.md#designPrototypeGetTags) | **GET** /Designs/{id}/tags | Queries tags of Design.
*DesignApi* | [**designPrototypeUpdateAttributesPatchDesignsid**](docs/DesignApi.md#designPrototypeUpdateAttributesPatchDesignsid) | **PATCH** /Designs/{id} | Patch attributes for a model instance and persist it into the data source.
*DesignApi* | [**designPrototypeUpdateAttributesPutDesignsid**](docs/DesignApi.md#designPrototypeUpdateAttributesPutDesignsid) | **PUT** /Designs/{id} | Patch attributes for a model instance and persist it into the data source.
*DesignApi* | [**designPrototypeUpdateByIdCategories**](docs/DesignApi.md#designPrototypeUpdateByIdCategories) | **PUT** /Designs/{id}/categories/{fk} | Update a related item by id for categories.
*DesignApi* | [**designPrototypeUpdateByIdTags**](docs/DesignApi.md#designPrototypeUpdateByIdTags) | **PUT** /Designs/{id}/tags/{fk} | Update a related item by id for tags.
*DesignApi* | [**designReplaceById**](docs/DesignApi.md#designReplaceById) | **POST** /Designs/{id}/replace | Replace attributes for a model instance and persist it into the data source.
*DesignApi* | [**designReplaceOrCreate**](docs/DesignApi.md#designReplaceOrCreate) | **POST** /Designs/replaceOrCreate | Replace an existing model instance or insert a new one into the data source.
*DesignApi* | [**designUpdateAll**](docs/DesignApi.md#designUpdateAll) | **POST** /Designs/update | Update instances of the model matched by {{where}} from the data source.
*DesignApi* | [**designUpsertPatchDesigns**](docs/DesignApi.md#designUpsertPatchDesigns) | **PATCH** /Designs | Patch an existing model instance or insert a new one into the data source.
*DesignApi* | [**designUpsertPutDesigns**](docs/DesignApi.md#designUpsertPutDesigns) | **PUT** /Designs | Patch an existing model instance or insert a new one into the data source.
*DesignApi* | [**designUpsertWithWhere**](docs/DesignApi.md#designUpsertWithWhere) | **POST** /Designs/upsertWithWhere | Update an existing model instance or insert a new one into the data source based on the where criteria.
*MessageApi* | [**messageGreet**](docs/MessageApi.md#messageGreet) | **GET** /Messages/greet | 
*TagApi* | [**tagCount**](docs/TagApi.md#tagCount) | **GET** /Tags/count | Count instances of the model matched by where from the data source.
*TagApi* | [**tagCreate**](docs/TagApi.md#tagCreate) | **POST** /Tags | Create a new instance of the model and persist it into the data source.
*TagApi* | [**tagCreateChangeStreamGetTagsChangeStream**](docs/TagApi.md#tagCreateChangeStreamGetTagsChangeStream) | **GET** /Tags/change-stream | Create a change stream.
*TagApi* | [**tagCreateChangeStreamPostTagsChangeStream**](docs/TagApi.md#tagCreateChangeStreamPostTagsChangeStream) | **POST** /Tags/change-stream | Create a change stream.
*TagApi* | [**tagDeleteById**](docs/TagApi.md#tagDeleteById) | **DELETE** /Tags/{id} | Delete a model instance by {{id}} from the data source.
*TagApi* | [**tagExistsGetTagsidExists**](docs/TagApi.md#tagExistsGetTagsidExists) | **GET** /Tags/{id}/exists | Check whether a model instance exists in the data source.
*TagApi* | [**tagExistsHeadTagsid**](docs/TagApi.md#tagExistsHeadTagsid) | **HEAD** /Tags/{id} | Check whether a model instance exists in the data source.
*TagApi* | [**tagFind**](docs/TagApi.md#tagFind) | **GET** /Tags | Find all instances of the model matched by filter from the data source.
*TagApi* | [**tagFindById**](docs/TagApi.md#tagFindById) | **GET** /Tags/{id} | Find a model instance by {{id}} from the data source.
*TagApi* | [**tagFindOne**](docs/TagApi.md#tagFindOne) | **GET** /Tags/findOne | Find first instance of the model matched by filter from the data source.
*TagApi* | [**tagPrototypeUpdateAttributesPatchTagsid**](docs/TagApi.md#tagPrototypeUpdateAttributesPatchTagsid) | **PATCH** /Tags/{id} | Patch attributes for a model instance and persist it into the data source.
*TagApi* | [**tagPrototypeUpdateAttributesPutTagsid**](docs/TagApi.md#tagPrototypeUpdateAttributesPutTagsid) | **PUT** /Tags/{id} | Patch attributes for a model instance and persist it into the data source.
*TagApi* | [**tagReplaceById**](docs/TagApi.md#tagReplaceById) | **POST** /Tags/{id}/replace | Replace attributes for a model instance and persist it into the data source.
*TagApi* | [**tagReplaceOrCreate**](docs/TagApi.md#tagReplaceOrCreate) | **POST** /Tags/replaceOrCreate | Replace an existing model instance or insert a new one into the data source.
*TagApi* | [**tagUpdateAll**](docs/TagApi.md#tagUpdateAll) | **POST** /Tags/update | Update instances of the model matched by {{where}} from the data source.
*TagApi* | [**tagUpsertPatchTags**](docs/TagApi.md#tagUpsertPatchTags) | **PATCH** /Tags | Patch an existing model instance or insert a new one into the data source.
*TagApi* | [**tagUpsertPutTags**](docs/TagApi.md#tagUpsertPutTags) | **PUT** /Tags | Patch an existing model instance or insert a new one into the data source.
*TagApi* | [**tagUpsertWithWhere**](docs/TagApi.md#tagUpsertWithWhere) | **POST** /Tags/upsertWithWhere | Update an existing model instance or insert a new one into the data source based on the where criteria.
*UserApi* | [**userConfirm**](docs/UserApi.md#userConfirm) | **GET** /Users/confirm | Confirm a user registration with email verification token.
*UserApi* | [**userCount**](docs/UserApi.md#userCount) | **GET** /Users/count | Count instances of the model matched by where from the data source.
*UserApi* | [**userCreate**](docs/UserApi.md#userCreate) | **POST** /Users | Create a new instance of the model and persist it into the data source.
*UserApi* | [**userCreateChangeStreamGetUsersChangeStream**](docs/UserApi.md#userCreateChangeStreamGetUsersChangeStream) | **GET** /Users/change-stream | Create a change stream.
*UserApi* | [**userCreateChangeStreamPostUsersChangeStream**](docs/UserApi.md#userCreateChangeStreamPostUsersChangeStream) | **POST** /Users/change-stream | Create a change stream.
*UserApi* | [**userDeleteById**](docs/UserApi.md#userDeleteById) | **DELETE** /Users/{id} | Delete a model instance by {{id}} from the data source.
*UserApi* | [**userExistsGetUsersidExists**](docs/UserApi.md#userExistsGetUsersidExists) | **GET** /Users/{id}/exists | Check whether a model instance exists in the data source.
*UserApi* | [**userExistsHeadUsersid**](docs/UserApi.md#userExistsHeadUsersid) | **HEAD** /Users/{id} | Check whether a model instance exists in the data source.
*UserApi* | [**userFind**](docs/UserApi.md#userFind) | **GET** /Users | Find all instances of the model matched by filter from the data source.
*UserApi* | [**userFindById**](docs/UserApi.md#userFindById) | **GET** /Users/{id} | Find a model instance by {{id}} from the data source.
*UserApi* | [**userFindOne**](docs/UserApi.md#userFindOne) | **GET** /Users/findOne | Find first instance of the model matched by filter from the data source.
*UserApi* | [**userLogin**](docs/UserApi.md#userLogin) | **POST** /Users/login | Login a user with username/email and password.
*UserApi* | [**userLogout**](docs/UserApi.md#userLogout) | **POST** /Users/logout | Logout a user with access token.
*UserApi* | [**userPrototypeCountAccessTokens**](docs/UserApi.md#userPrototypeCountAccessTokens) | **GET** /Users/{id}/accessTokens/count | Counts accessTokens of User.
*UserApi* | [**userPrototypeCreateAccessTokens**](docs/UserApi.md#userPrototypeCreateAccessTokens) | **POST** /Users/{id}/accessTokens | Creates a new instance in accessTokens of this model.
*UserApi* | [**userPrototypeDeleteAccessTokens**](docs/UserApi.md#userPrototypeDeleteAccessTokens) | **DELETE** /Users/{id}/accessTokens | Deletes all accessTokens of this model.
*UserApi* | [**userPrototypeDestroyByIdAccessTokens**](docs/UserApi.md#userPrototypeDestroyByIdAccessTokens) | **DELETE** /Users/{id}/accessTokens/{fk} | Delete a related item by id for accessTokens.
*UserApi* | [**userPrototypeFindByIdAccessTokens**](docs/UserApi.md#userPrototypeFindByIdAccessTokens) | **GET** /Users/{id}/accessTokens/{fk} | Find a related item by id for accessTokens.
*UserApi* | [**userPrototypeGetAccessTokens**](docs/UserApi.md#userPrototypeGetAccessTokens) | **GET** /Users/{id}/accessTokens | Queries accessTokens of User.
*UserApi* | [**userPrototypeUpdateAttributesPatchUsersid**](docs/UserApi.md#userPrototypeUpdateAttributesPatchUsersid) | **PATCH** /Users/{id} | Patch attributes for a model instance and persist it into the data source.
*UserApi* | [**userPrototypeUpdateAttributesPutUsersid**](docs/UserApi.md#userPrototypeUpdateAttributesPutUsersid) | **PUT** /Users/{id} | Patch attributes for a model instance and persist it into the data source.
*UserApi* | [**userPrototypeUpdateByIdAccessTokens**](docs/UserApi.md#userPrototypeUpdateByIdAccessTokens) | **PUT** /Users/{id}/accessTokens/{fk} | Update a related item by id for accessTokens.
*UserApi* | [**userReplaceById**](docs/UserApi.md#userReplaceById) | **POST** /Users/{id}/replace | Replace attributes for a model instance and persist it into the data source.
*UserApi* | [**userReplaceOrCreate**](docs/UserApi.md#userReplaceOrCreate) | **POST** /Users/replaceOrCreate | Replace an existing model instance or insert a new one into the data source.
*UserApi* | [**userResetPassword**](docs/UserApi.md#userResetPassword) | **POST** /Users/reset | Reset password for a user with email.
*UserApi* | [**userUpdateAll**](docs/UserApi.md#userUpdateAll) | **POST** /Users/update | Update instances of the model matched by {{where}} from the data source.
*UserApi* | [**userUpsertPatchUsers**](docs/UserApi.md#userUpsertPatchUsers) | **PATCH** /Users | Patch an existing model instance or insert a new one into the data source.
*UserApi* | [**userUpsertPutUsers**](docs/UserApi.md#userUpsertPutUsers) | **PUT** /Users | Patch an existing model instance or insert a new one into the data source.
*UserApi* | [**userUpsertWithWhere**](docs/UserApi.md#userUpsertWithWhere) | **POST** /Users/upsertWithWhere | Update an existing model instance or insert a new one into the data source based on the where criteria.


## Documentation for Models

 - [AccessToken](docs/AccessToken.md)
 - [Category](docs/Category.md)
 - [Customer](docs/Customer.md)
 - [Design](docs/Design.md)
 - [InlineResponse200](docs/InlineResponse200.md)
 - [InlineResponse2001](docs/InlineResponse2001.md)
 - [InlineResponse2002](docs/InlineResponse2002.md)
 - [InlineResponse2003](docs/InlineResponse2003.md)
 - [Tag](docs/Tag.md)
 - [User](docs/User.md)


## Documentation for Authorization

Authentication schemes defined for the API:
### access_token

- **Type**: API key
- **API key parameter name**: access_token
- **Location**: URL query string


## Recommendation

It's recommended to create an instance of `ApiClient` per thread in a multithreaded environment to avoid any potential issues.

## Author



