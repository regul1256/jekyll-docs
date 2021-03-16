# Creating a Portal signal watcher 
Complete this task to create a signal watcher. 

A signal watcher is a tool that allows monitoring of tag values via setting different conditions. You can create complex conditions that include several tags from different projects. Read the [Signal Watchers](../2-Portal/portal_swatchers.md) article for details. 

1. In the Signal Watchers section, click the **Add new Signal Watcher** ![swatcher.md](images/swatcher.png) button.
2. Type the signal watcher name and name in the **Title** and **Message** fields.
3. Set the signal watcher activation delay with the **Delay-On** setting.
4. Set the signal watcher deactivation delay with the **Delay-Off** setting. 

    <figure>
       <img src="../images/delays.png" alt="Settings section">
       <figcaption><b>Figure 1.</b> Setting signal watcher activation and deactivation delays</figcaption>
    </figure>

    !!! note
        By default, delays are enabled. If you do not need delays for your signal watcher, put the **Enabled** flag off. 

5. Choose the way of the signal watcher occurrence: 
    
    - **All**<br>
    A signal watcher is active only if all the conditions were met.
    - **Any**<br>
    A signal watcher is active if at least one of the conditions was met.

6. Click **Add condition** and set the following parameters: 

    - Project
    - Tag
    - Operator
    - Type 
    - Set limit/Offset


    <figure>
       <img src="../images/delays.png" alt="Settings section">
       <figcaption><b>Figure 2.</b> Configuring Conditions</figcaption>
    </figure>

    !!! important
        You can add as many conditions as you need. By default, the way **All** is set. 

***
**Related article:** 

- **[Signal Watchers](../2-Portal/portal_swatchers.md)**<br>
Signal Watchers is the section of Portal where you can create, modify and observe signal watchers. 