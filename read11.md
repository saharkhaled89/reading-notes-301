
# Working with volumes

## Performing a search

**You can perform a volumes search by sending an HTTP GET request to the following URI:**

**https://www.googleapis.com/books/v1/volumes?q=search+terms**

**This request has a single required parameter:**

## q - Search for volumes that contain this text string. There are special keywords you can specify in the search terms to search in particular fields, such as:

* intitle: Returns results where the text following this keyword is found in the title.

* inauthor: Returns results where the text following this keyword is found in the author.

* inpublisher: Returns results where the text following this keyword is found in the publisher.

* subject: Returns results where the text following this keyword is listed in the category list of the volume.

* isbn: Returns results where the text following this keyword is the ISBN number.

* lccn: Returns results where the text following this keyword is the Library of Congress Control Number.

* oclc: Returns results where the text following this keyword is the Online Computer Library Center number.

# Filtering

**You can use the filter parameter to restrict the returned results further by setting it the to one of the following values:**

* partial - Returns results where at least parts of the text are previewable.

* full - Only returns results where all of the text is viewable.

* free-ebooks - Only returns results that are free Google eBooks.

* paid-ebooks - Only returns results that are Google eBooks with a price.

* ebooks - Only returns results that are Google eBooks, paid or free. Examples of non-eBooks would be publisher content that is available in limited preview and not for sale, or magazines.

# Query parameter reference

**The query parameters you can use with the Books API are summarized in this section.  All parameter values need to be URL encoded.**

## Standard query parameters

**Query parameters that apply to all Books API operations are shown in the table below.**

**Notes (on API keys and auth tokens):**

* *The key parameter is required with every request, unless you provide an OAuth 2.0 token with the request.*

* *You must send an authorization token with every request that requires an OAuth scope. OAuth 2.0 is the only supported authorization protocol.*

* **You can provide an OAuth 2.0 token with any request in one of two ways:**

* *Using the access_token query parameter like this: ?access_token=oauth2-token*

* *Using the HTTP Authorization header like this: Authorization: Bearer oauth2-token*


# What is EJS?

 **EJS is a simple templating language that lets you generate HTML markup with plain JavaScript. No religiousness about how to organize things. No reinvention of iteration and control-flow. It's just plain JavaScript.**


## **Install**

**It's easy to install EJS with NPM.**

**$ npm install ejs**

![img](/img/option.png)




