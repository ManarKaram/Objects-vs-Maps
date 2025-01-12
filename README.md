
# Objects vs Maps


## Table of content

- The concepts ( what's Map and Object? )
- Differences between Map and Object
- Usage of them

  - How to construct?
  - Accessing elements
  - Adding new elements
  - Checking if element is exist
  - Removing element
  - Checking the size
  - Iterating

- Conclusion


What's Map and Object?

  Map:

  - Map is a data collection type (_abstract data structure type_), in which, data is stored in a form of  **pairs** , which contains a  **unique**   **key**  and  **value mapped to that key**. And because of the uniqueness of each stored key, there is  **no duplicate**  pair stored.
  - Map is mainly used for  **fast searching and looking up**  data.

  Object:

  - Object is object (_ **Regular** _** Object),** _type_ of data collection, which means it also  **follows key-value stored concept**  like Map. Each  **key**  in Object or we normally call it "property" which is also  **unique**  and  **associated with a single value**.
  - Object in JavaScript has  **built-in prototype** and is used **to manipulate values an combine them into more complex objects**.

Differences between Map and Object

  | Map | Object |
  | --- | --- |
  | the key-field can be of any data-type (integer, an array, even an object!) | the data-type of the key-field is restricted to integer, strings, and symbols |
  | the original order of elements is preserved | the original order of elements isn't preserved |
  | Map is an instance of an object | Object isn't an instance of map but is instance of classes |
  | Json don't support maps | Json support objects |

Usage of them
How to construct?
  
  **Map:**

      Map is constructed and declared by using its built-in constructor and _new_ syntax.
      
![image](https://user-images.githubusercontent.com/59695197/199068949-76de1704-dbfd-44b2-850b-b7bda04ab65f.png)


   **Object:**

      Object has several ways to declare.

      -Direct literal
      
![image](https://user-images.githubusercontent.com/59695197/199069115-8c1afb43-7890-454b-b76b-793ff850a83c.png)


      -by constructor
![image](https://user-images.githubusercontent.com/59695197/199069199-f271f65c-8f19-48c3-b430-94b4817324e0.png)


      -by using _ **Object.prototype.create** _
![image](https://user-images.githubusercontent.com/59695197/199069280-091f7e00-70ad-44ca-b087-ae4dca43c2a9.png)

      -by using **built-in constructor**
![image](https://user-images.githubusercontent.com/59695197/199069439-1a30a872-73a7-44e6-b6ca-a998e5f8c03e.png)


  Accessing elements

   **Map:** Map uses its inbuilt **get() method** for accessing its elements.
![image](https://user-images.githubusercontent.com/59695197/199069736-d5be9d4c-56d6-447b-bf5f-778fb823938e.png)


   **Object:** Objectsimply uses the _'key'_ name with a dot **(.) operator** to access its elements.
![image](https://user-images.githubusercontent.com/59695197/199069852-3711e86d-fb40-4c02-a525-da40ac1c030d.png)


  Adding new elements

   **Map:** Map uses **set() method** to add new element.
![image](https://user-images.githubusercontent.com/59695197/199069921-5d7f0103-634e-4972-a120-0b93ec31408e.png)

   **Object:**  it is done directly.
![image](https://user-images.githubusercontent.com/59695197/199069991-4544eb3f-6d67-4706-8a89-b17e24908a62.png)


  Checking if element is exist

   **Map:** Map uses it's **inbuilt has() method** for this.
![image](https://user-images.githubusercontent.com/59695197/199070068-feeba5c4-391b-4648-baa6-b8cfe3b57f0d.png)


   **Object:**  Object uses **'===' operator** for performing the task.
 ![image](https://user-images.githubusercontent.com/59695197/199070186-889b9819-2437-4743-9282-8b32baa9f86e.png)



Removing element

  **Map:**

   **-Delete item.**

      Map uses it's **inbuilt** **delete()** that returns a Boolean value.
![image](https://user-images.githubusercontent.com/59695197/199073315-26bcaa1b-2d70-412c-9327-cc3d0be5cc5a.png)

   **-Delete MapSet.**

      Map uses it's **inbuilt** **clear()** that will remove all Map elements.
![image](https://user-images.githubusercontent.com/59695197/199073359-7f183ea4-9c1e-48b7-a861-63ceb7e0df31.png)

  **Object:**  
      there is no built-in method to delete a property from it. Instead, we can use the operator  **delete**.
![image](https://user-images.githubusercontent.com/59695197/199073589-6288e8b2-f43f-4b32-8091-dcc937c92387.png)
![image](https://user-images.githubusercontent.com/59695197/199073623-0dd68223-50bd-4b96-a294-c14b7851bd62.png)

      Or we can **" undefine "** the element itself as follows:
![image](https://user-images.githubusercontent.com/59695197/199073676-9cdc6627-092e-49de-97d6-50902d2b6aa0.png)



Checking the size

  **Map:** Map automatically updates its size and get the easiest.
![image](https://user-images.githubusercontent.com/59695197/199073801-293ed37e-3a9d-4f8d-b66f-4bb8d1c2e864.png)


  **Object:**  it needs to be calculated manually, with the help of _**Object.keys()**_

![image](https://user-images.githubusercontent.com/59695197/199073862-7f5cf9ff-36dd-4a32-86d1-d72c926857cd.png)



Iterating

  **Map:** is built-in iterable.
  
![image](https://user-images.githubusercontent.com/59695197/199073973-daa8e28d-1044-4c2b-b998-fb5a50f53fc1.png)



  **Object**** : **either we use**" **_** for… in **_**" **Or using ** Object.keys(obj)** to get all the keys and iterate

![image](https://user-images.githubusercontent.com/59695197/199074011-474729db-6295-4836-add1-822c10824fab.png)

![image](https://user-images.githubusercontent.com/59695197/199074042-2942ced7-5ce8-4654-a852-0d1ddb100421.png)


Conclusion

      Despite all the advantages  **Map**  can have against  **Object** , there is still cases  **Object**  will perform better. After all, Object is the most basic    concept of Javascript.

      - Objects are a great choice for situations where we need simple structure to store data and the type of keys needed is either an integer, strings or symbols.
      - Scenarios which needs the application of separate logic to individual property element, the object is definitely the choice.
      - Map is completely hash whereas Object is more than that.

      Map tends to have more advantages over  **Object**  in scenarios when we just need a simple look-up structure for data storing, with all the basic operations it provided. However,  **Map**  can't never replace  **Object** , in any sense, because in Javascript,  **Object**  is — after all —  **more than just**  a normal hash table (_and therefore shouldn't be used as a normal hash table if there is alternative, it's just a waste of a great resource ;)_).


