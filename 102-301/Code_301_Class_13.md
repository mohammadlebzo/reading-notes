# Reading 13

## Status Codes Based On REST Methods

1. *In your own words, describe what each group of status code represents*:
    - 100’s = they are **informational status code**, which tells the *client* that the **header of the request was received** but it's **going to fail** before sending the *body*.
    - 200’s = they are **success codes**, which *informs* the *client* that the *request* was **accepted**, *but* it **doesn't** mean that it was **processed successfully**.
    - 300’s = they are **redirection codes**, which *informs* the *client* that whatever they are *requesting* **isn't available** at the **URL/location** they entered.
    - 400’s = they are **error codes**, which means that what the **client is sendeing isn't correct**, and **should be checked before re-entering**.
    - 500’s = they are **server error codes**, which *informs* the *client* that the **server might be unreachable or facing problems**.
2. *What is a status code 202*? [source](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/202)

**The request has been accepted for processing, but the processing has not been completed**.

3. *What is a status code 308*? [source](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/308)

**The resource requested has been definitively moved to the URL given by the Location headers**.

4. *What code would you use if an update didn’t return data to a client*? *code*: **204**
5. *What code would you use if a resource used to exist but no longer does*? *code*: **308**
6. *What is the ‘Forbidden’ status code*? *code*: **403**

## Build A REST API With Node.js, Express, & MongoDB - Quick

1. *Why do we need to pull our MongoDB database string out of our server and put it into our .env*?

Because when *using* the **application** we will use a **different string that the local host**.

2. *What is middleware*? it a **software** that **provieds additional services** to **other softwares**.

3. *What does `app.use(express.json())` do*? it allows the *database* to **accept JSON** in the **body**.

4. *What does the `/:id` mean in a route*? **it means that this is a parameter**.

5. *What is the difference beween `PUT` and `PATCH`*? `PUT` *replaces* the **entire resource** with given data, while `PATCH` *replaces* **only specified**.

6. *How do you make a defalut value in a schema*? **by giving it a default parameter**.

7. *What does a `500` error status code mean*? **generic error response**.

8. *What is the difference between a status `200` and a status `201`*?

*code*: **200** = *request* was **received** and is **being processed**, but *code*: **201** = *request* was **successful** and a **resource has been created**.

## Things I want to know more about

None.
