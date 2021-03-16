# Use writable scripts
This example shows you how to create a virtual tag with the writable script.  
## What is a writable script? 
A writable script is a script of virtual tags which allows changing of a particular element in an array data type tag. You can find the Writable script field in the [Virtual tag editor](../4-IDE/vt_ed.md). 

The mechanism of changing an array's element consists of two parts: 

1. The **readable script** is a part where a virtual tag reads an element from a tag that returns an array of values. 
2. The **writable script** is a part responsible for changing the element's value in the mentioned above tag.

The readable script uses the expression:
```
value(pathToTag) [element's index]. 
```
The writable script's work is based on two functions:

1. `inputValue ()`function returns the input value for the writable virtual tag.
2. `writeSingleValueToArray(tagPath, value, index)` function writes the value that has been returned by inputValue() function to the tag element with defined index. 

    !!! important
        The indexes in the readable and the writable scripts should match.

## Creating a writable script
### Prerequisites
You will need the following to complete this task: 

- An array type tag
- A virtual tag. 

### Steps 

1. Create a virtual tag or use the existing one. <!--Here can be a reference to an instruction for creating a virtual tag-->
2. Put into the **Readable script** field the following expression: 

    ```
    value("folder/deviceName/tagName") [index (number of an array element)]
    ```
    !!! important
        Array indexes start with **"0"**, so the first element of an array has number 0. 

3. Put into the **Writable script** field the following expression: 

    ```
    writeSingleValueToArray("folder/deviceName/tagName", inputValue(), index)
    ```

4. Click Save. 

### Checking the result
As a result of these operations, you will have a virtual tag which can change one element of an array tag on your demand. If anything is correct, then you will see the tag's current value in the square brackets. 

After creating the virtual tag with the writable script, you can create a page element, for example a button, which will change the tag value on click. <!--I should put the reference to the task for creating such button.--> 

***
**Related articles**: 

- **[Virtual tag editor](../4-IDE/vt_ed.md)**<br>
Editing virtual tags.
- **[View tags](../2-Portal/Projects_view_tags.md)**<br>
You can read about settings of tags and alarms in this article.