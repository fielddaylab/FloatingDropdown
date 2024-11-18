# FloatingDropdown
Simple reusable web component for web games linking to the Vault

## Example
This example illustrates how this component can be added to a project

### Step 1: Add custom component to the header of the index file

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
