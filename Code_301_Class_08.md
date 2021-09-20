# Reading 08

## API Design Best Practices

1. *What does REST stand for*? 

It stands for **Representational State Transfer**.

2. *REST APIs are designed around a ____*. 

REST APIs are designed around a **resource**.

3. *What is an identifer of a resource? Give an example*. [source](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

**ex**: *https://adventure-works.com/orders/1*

4. *What are the most common HTTP verbs*?

**The most common HTTP verbs are**:

- `GET`
- `POST`
- `PUT`
- `PATCH`
- `DELETE`

5. *What should the URIs be based on*?

**URIs** should be *based* on **nouns** and not **verbs**.

6. *Give an example of a good URI*. [source](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

**ex**: *https://adventure-works.com/orders*

7. *What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing*?

It means that there will be a **larg number of small resources for the API**, which will *result* in **load on the server**

8. *What status code does a successful `GET` request return*?

It *returns* an **HTTP status code 200 (OK)**.

9. *What status code does an unsuccessful `GET` request return*?

It *returns* a **404 (Not Found)**.

10. *What status code does a successful `POST` request return*?

It *returns* an **HTTP status code 201 (Created)**.

11. *What status code does a successful `DELETE` request return*?

It *returns* an **HTTP status code 204 (No Content)**.

## Things I want to know more about

None.
