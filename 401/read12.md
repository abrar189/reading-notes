## Spring RequestMapping

## @RequestMapping Basics :

- @RequestMapping — by Path

1. define the Request URI to access the REST Endpoints
2. @RequestMapping(value = "/ex/foos", method = RequestMethod.GET)

- @RequestMapping — the HTTP Method

1. The HTTP method parameter has no default
2. @RequestMapping(value = "/ex/foos", method = POST) @ResponseBody

- RequestMapping and HTTP Headers

1. @RequestMapping With the headers Attribute

- The mapping can be narrowed even further by specifying a header for the request:

@RequestMapping(value = "/ex/foos", headers = "key=val", method = GET)
  @ResponseBody

2. @RequestMapping Consumes and Produce

@RequestMapping(
  value = "/ex/foos",
  method = GET,
  headers = "Accept=application/json")
  @ResponseBody

## RequestMapping With Path Variables

- Parts of the mapping URI can be bound to variables via the @PathVariable annotation.

1. Single @PathVariable
2. Multiple @PathVariable
3. @PathVariable With Regex

## RequestMapping With Request Parameters

- allows easy mapping of URL parameters with the @RequestParam annotation.

## CrudRepository, JpaRepository, and PagingAndSortingRepository in Spring Data

- CrudRepository provides CRUD functions.

- PagingAndSortingRepository provides methods to do pagination and sort records.

- JpaRepository provides JPA related methods such as flushing the persistence context and delete records in a batch.

- Implement a simple operation: @Repository public interface ProductRepository extends JpaRepository<Product, Long> { Product findByName(String productName); }

## CRUD functionality:

1. save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch.

2. findOne(…) – get a single entity based on passed primary key value.

3. findAll() – get an Iterable of all available entities in database.

4. count() – return the count of total entities in a table.

5. delete(…) – delete an entity based on the passed object.

6. exists(…) – verify if an entity exists based on the passed primary key value.