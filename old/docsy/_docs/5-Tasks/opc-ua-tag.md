# Create an OPC UA tag
After completing this task, you will be able to create OPC UA tags. 

1. Enter the [OPC UA device](opc-ua-dev.md). 
2. Click the **Create OPC UA tag** ![opc-tag.png](images/opc-tag.png) icon. You will see the following menu. 

    <figure>
      <img src="../images/opc-tag-menu.png" alt="Tag configuration menu">
      <figcaption><b>Figure 1.</b> Tag configuration menu</figcaption>
    </figure>

3. Name the tag in the **Tag name** field, and set the **Custom name** and **Description** if necessary. 

    !!! important
        It is obligatory to fill the **Tag name** field. 

4. Configure **OPC UA settings** in the same-named section. 

    4.1. Set the device's address: `ns=2;s=1:FC1001?SetPoint`. Where: 

    - `ns=2;s=1:` is the NodeId
    - `FC1001?SetPoint`are device and tag names.

    !!! note
        Read **OPC Unified Architecture Specification Part 3: Address Space Model** for more information about addressing model of OPC UA.  

    4.2. Set the request interval so the device would request data from the tag every 5 seconds. 

***

**Related articles:**

- **[OPC UA devices](../4-IDE/opc_dev.md)**<br>
OPC UA devices and their parameters.
- **[OPC UA tag editor](../4-IDE/opc_ed.md)**<br>
This article is about OPC UA tags and their parameters which you can change in the editor.
- **[Tag general settings](../4-IDE/tag_gen_settings.md)**<br>
In this article, you can find short descriptions of tag general settings.
- **[Tag history settings](../4-IDE/history_set.md)**<br>
Briefly about History settings menu.
- **[View tags](../2-Portal/Projects_view_tags.md)**<br>
You can read about settings of tags and alarms in this article.

**Related task**

- **[Create an OPC UA device](opc-ua-dev.md)**<br>
This task will help you with creating an OPC UA device.
    