# FloatingDropdown
Simple reusable web component for web games linking to the [Vault](https://vault.fielddaylab.wisc.edu/)

This repository houses a reusable html component for the Vault floating dropdown on free browser-based games. There are two pieces used for this component: 
1. the html template used to display the component on the dom 
2. the Unity javascript plugin to be used to remove the buttom after exitting the title screen.

## 1. Adding the Component
This example illustrates how this component can be added to a project

### Step 1: Add a custom component to the header of the index file

```javascript
<script src="FloatingDropdown/index.js"></script>
```

### Step 2: Add the custom element to the body of the file

This element uses ***slots*** to make the component more flexible. If you are unfamiliar with slots, you can read more [here](https://developer.mozilla.org/en-US/docs/Web/API/Web_components/Using_templates_and_slots#adding_flexibility_with_slots)

Example from a Unity WebGL Template:
```javascript
<body>
    <div id="BrainPOPsnapArea">
        <div class="webgl-content">
            /* Here is the floating dropdown component */
            <floating-dropdown>
                <style> /* Add custom fonts here */ </style>
                <img slot="header" src="/path/to/header/image" alt="Vault Games Library" width="250px">
                <p slot="desc" class="content" style="font-weight: 400;">
                    Put the body text here
                </p>
                <p slot="button-label" class="content" style="font-weight: bolder;">
                    Put button label here
                </p>
            </floating-dropdown>
...

```
